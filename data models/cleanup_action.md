## Object: cleanup_action

Represents actions taken during environmental cleanup events. Users can report completed actions with descriptions and photos.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'cleanup_action' in this case.    | String 'cleanup_action' | No   | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| project_id        | ID of the associated project                                        | integer             | No     | Yes      |
| user_id           | ID of the user who performed the cleanup action                     | integer             | No     | Yes      |
| location          | Geographical location of the cleanup action                         | string              | No     | Yes      |
| action_date       | Date and time the action was performed                              | datetime            | No     | Yes      |
| description       | Description of the cleanup action                                  | string              | No     | Yes      |
| photos            | Media files associated with the cleanup action                     | string (URL)        | No     | No       |