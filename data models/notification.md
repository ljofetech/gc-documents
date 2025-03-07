## Object: notification

Represents notifications sent to users to alert them of new activities, pollution updates, or other events.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'notification' in this case.      | String 'notification' | No    | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| user_id           | ID of the user receiving the notification                          | integer             | No     | Yes      |
| message           | Content of the notification                                        | string              | No     | Yes      |
| type              | Type of notification (e.g., new polluted area, update, event)      | string              | No     | Yes      |
| read_status       | Whether the notification has been read by the user                 | boolean             | No     | Yes      |
| created_at        | Date and time the notification was created                         | datetime            | No     | Yes      |