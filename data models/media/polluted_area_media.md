## Object: polluted_area_media

Stores media (photos, videos) linked to a polluted area to provide visual evidence of pollution.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'polluted_area_media' in this case. | String 'polluted_area_media' | No | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| polluted_area_id  | ID of the polluted area associated with the media                  | integer             | No     | Yes      |
| media_type        | Type of media (e.g., photo, video, document)                       | string              | No     | Yes      |
| url               | URL link to the media file                                          | string (URL)        | No     | Yes      |
| description       | Description of the media file (e.g., photo caption)                | string              | No     | No       |