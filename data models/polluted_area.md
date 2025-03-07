## Object: polluted_area

Represents a polluted area in Cyprus. Each polluted area is associated with a pollution type, severity, and geolocation.

| Naming            | Description                                                        | Type                | Unique | Required |
|-------------------|--------------------------------------------------------------------|---------------------|--------|----------|
| object_type       | The type of the object, which is 'polluted_area' in this case.     | String 'polluted_area' | No   | Yes      |
| **Attributes (data)** |                                                             |                     |        |          |
| type_of_pollution | Type of pollution (air, water, soil, waste)                        | string              | No     | Yes      |
| pollution_level   | Level of pollution (low, medium, high)                             | string              | No     | Yes      |
| description       | Detailed description of the pollution                              | string              | No     | No       |
| location          | Geographical location of the polluted area                         | string              | No     | Yes      |
| created_at        | Date and time the polluted area was added to the system            | datetime            | No     | Yes      |
| updated_at        | Date and time the polluted area data was last updated             | datetime            | No     | Yes      |