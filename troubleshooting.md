# Troubleshooting

Below are some common issues associated with the Impersonate B2, and some suggestions in regard to identifying the root cause of the problem.

### Taken to the homepage after clicking impersonate?

If you haven't yet entered a user's username, this is caused by not having sufficient privlidges to access the Building Block. You have the correct entitlements, but something else is not quite right. If you have just been granted the entitlement, or had your system role changed, try logging out and then back in. If you have just installed or upgraded the Building Block, restart the app server to ensure the correct version of the Building Block has been loaded.

### Taken to the homepage after executing an impersonate?

If you have only been granted the **Administrator Panel \(Tools and Utilities\) &gt; Impersonate User w/ Less than or Equal Role** entitlement, this means that you are tying to impersonate a user with a greater role than you currently have. The logs should also include a message like `Impersonate User Level Check FAILED` indicating this.

### Taken to a blank after executing an impersonate?

The user you are trying to impersonate doesn't exist, or the B2 experienced an issue binding your current session to the desired user. If you are sure that the user exists, logging out and back in again may fix the problem. If the issue persists, the [log file](/logs.md) might be of use to you.

