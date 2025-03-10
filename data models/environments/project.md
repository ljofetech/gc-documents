## Object: project

A project represents an environmental initiative on the platform, such as a cleanup effort or awareness campaign. It can be created by individuals or organizations.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'project' in this case.           | String 'project'    | No     | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| title             | Title of the project                                               | string              | No     | Yes      |
| description       | Detailed description of the project                                | string              | No     | Yes      |
| created_by        | User ID of the creator (volunteer or organization)                 | integer             | No     | Yes      |
| status            | Current status of the project (active, completed, etc.)            | string              | No     | Yes      |
| location          | Geographical location of the project                               | string              | No     | No       |
| start_date        | Date when the project starts                                        | datetime            | No     | Yes      |
| end_date          | Date when the project ends                                          | datetime            | No     | No       |
| created_at        | Date and time when the project was created                          | datetime            | No     | Yes      |
| updated_at        | Date and time when the project data was last updated               | datetime            | No     | Yes      |