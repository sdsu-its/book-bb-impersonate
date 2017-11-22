# Granting Impersonate Privileges  

Impersonate uses the Blackboard Entitlements model to determine whether or not to allow a user to impersonate a given user. Two discreete entitlements are avalible in the 

* Administrator Panel \(Tools and Utilities\) &gt; Impersonate Any User
* Administrator Panel \(Tools and Utilities\) &gt; Impersonate User w/ Less than or Equal Role

Role relationships are determined via the number of entitlements associated with a given user's role. For example, a user with no system role, like an instructor or student would have 0 entitlements; whereas a system administrator would have hundreds of entitlements. While not 100% bulletproof, this ensures that users cannot impersonate a user higher than them to change their access level.



