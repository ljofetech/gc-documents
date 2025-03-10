## Object: Achievement

An achievement represents a milestone or recognition earned by a user within the platform.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'achievement' in this case.       | String 'achievement'| No     | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| name              | Name or title of the achievement                                    | string              | No     | Yes      |
| description       | Detailed description of the achievement                            | string              | No     | Yes      |
| points            | Points or value associated with the achievement                    | integer             | No     | No       |
| achievement_type  | The category or type of the achievement (e.g., environmental, task) | string              | No     | No       |
| badge_image       | URL link to an image or badge representing the achievement         | string (URL)        | No     | No       |
| created_at        | Date and time when the achievement record was created              | datetime            | No     | Yes      |
| updated_at        | Date and time when the achievement record was last updated        | datetime            | No     | Yes      |