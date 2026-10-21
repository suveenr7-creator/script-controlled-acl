# Phase 8: Create the Delete ACL and Verify the Project

## Steps
1. Open **System Security > Access Control (ACL)** and click **New**.
2. Configure:
   - Type: `record`
   - Operation: `delete`
   - Name: `u_institution_details`
   - Active: `true`
3. In the **Requires role** related list, add `bb4`.
4. Do not add a data condition, as specified in the project PDF.
5. Save the ACL.
6. Test with a user who has all four roles: `bb1`, `bb2`, `bb3`, and `bb4`.
7. Verify the expected permissions:
   - `bb1`: read access
   - `bb2`: create access
   - `bb3`: write/edit access
   - `bb4`: delete access
8. Confirm that the final behavior matches the project PDF's outcome: ACLs control viewing, creating, editing and deleting records.

## Video narration
"Finally, I create the Delete ACL requiring bb4. I test the user with all four roles and review the Read, Create, Write and Delete permissions."

## Result
The project includes a custom table, test data, and Read, Create, Write and Delete ACLs.

## Closing line for the video
"This completes the Script-Controlled ACL project. The roles and ACL rules are used to control access to Institution Details records. Thank you for watching."

**Important source note:** These phases are organized from the uploaded PDF. Test the ACLs in your ServiceNow instance; actual behavior depends on the configured ACL rules and platform evaluation.
