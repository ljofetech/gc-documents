## Object: complaint

Represents a complaint related to pollution or environmental issues. Users can report concerns, issues, or incidents of pollution, including details and supporting media.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'complaint' in this case.          | String 'complaint'   | No     | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| project_id        | ID of the associated project                                        | integer             | No     | Yes      |
| user_id           | ID of the user filing the complaint                                 | integer             | No     | Yes      |
| location          | Geographical location where the complaint was reported              | string              | No     | Yes      |
| complaint_date    | Date and time the complaint was filed                               | datetime            | No     | Yes      |
| description       | Detailed description of the complaint                               | string              | No     | Yes      |
| status            | Current status of the complaint (e.g., open, resolved, etc.)        | string              | No     | Yes      |
| priority          | Priority level of the complaint (e.g., high, medium, low)           | string              | No     | No       |
| photos            | Media files associated with the complaint                           | string (URL)        | No     | No       |
