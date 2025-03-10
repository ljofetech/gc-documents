## Object: user

A user represents an individual or an organization using the platform. They can be regular users, volunteers, or environmental organizations contributing to the project.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'user' in this case.              | String 'user'       | No     | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| name              | User's full name                                                   | string              | No     | Yes      |
| email             | User's email address                                               | string (email)      | Yes    | Yes      |
| password          | Encrypted password for user authentication                        | string (encrypted)  | No     | Yes      |
| role              | Role of the user (e.g., regular, volunteer, organization)          | string              | No     | Yes      |
| location          | Geographical location of the user                                  | string              | No     | No       |
| profile_picture   | URL link to the user's profile picture                             | string (URL)        | No     | No       |
| created_at        | Date and time when the user account was created                    | datetime            | No     | Yes      |
| updated_at        | Date and time when the user data was last updated                  | datetime            | No     | Yes      |