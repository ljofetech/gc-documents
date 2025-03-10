# Interaction between Entities

The entities within the database interact with each other in several ways to form a fully functioning platform for environmental monitoring and volunteer participation. Below is an explanation of how each entity connects and interacts within the system.

---

## 1. **User** ↔ **Project**  
Users create and manage **Projects**, which can be an environmental initiative, such as a cleanup event or awareness campaign. Users can register as individuals, volunteers, or organizations and take part in existing projects. **Users** can interact with **Projects** by joining them, contributing, or reporting on them.

- **User**: A volunteer or organization creates or participates in a **Project**.
- **Project**: Contains details about the initiative and is linked to **Users** who contribute to or manage it.

---

## 2. **Project** ↔ **PollutedArea**  
**Projects** often aim to address pollution in specific regions. Therefore, the **PollutedArea** entity is tied to **Projects**, as cleanups or interventions can be organized in these polluted locations. **PollutedAreas** can be associated with **Projects** by being identified as the target for cleanup.

- **Project**: Initiates or organizes an environmental activity aimed at cleaning specific **PollutedAreas**.
- **PollutedArea**: Areas marked on the map where pollution is high and are targeted by **Projects**.

---

## 3. **PollutedArea** ↔ **PollutionMeasurement**  
Each **PollutedArea** can have multiple pollution measurements, which are taken by sensors or users. **PollutionMeasurements** provide real-time data for the pollution level in each **PollutedArea** (e.g., air quality, water toxicity, etc.).

- **PollutedArea**: Represents a specific location with pollution.
- **PollutionMeasurement**: Provides data on pollution levels for each **PollutedArea**, updated regularly.

---

## 4. **PollutedArea** ↔ **PollutedAreaMedia**  
Visual proof of pollution is crucial for environmental monitoring. **PollutedAreaMedia** stores media files (images, videos, etc.) of the polluted areas to provide visual evidence of the pollution. These media files are associated with specific **PollutedAreas**.

- **PollutedArea**: The location affected by pollution.
- **PollutedAreaMedia**: Media files (photos, videos) linked to specific **PollutedAreas** for documentation.

---

## 5. **PollutedArea** ↔ **Notification**  
Users receive **Notifications** about new polluted areas, changes in pollution levels, or actions to be taken. These notifications are triggered by updates related to **PollutedAreas**.

- **PollutedArea**: When new polluted areas are identified or updated, **Users** are notified.
- **Notification**: Alerts users about new **PollutedAreas**, pollution updates, or related actions.

---

## 6. **User** ↔ **CleanupAction**  
Users can perform **CleanupActions** as part of projects, and report these actions once they are completed. **CleanupActions** are actions like waste collection, removing hazardous materials, or restoring polluted areas. Users can upload media and descriptions to these actions.

- **User**: A volunteer or an organization executes a **CleanupAction**.
- **CleanupAction**: Represents the cleanup activity performed by **Users** in **PollutedAreas**.

---

## 7. **CleanupAction** ↔ **PollutedArea**  
Each **CleanupAction** is related to a specific **PollutedArea**. The goal of the action is to reduce pollution in the identified area. **CleanupActions** are linked to **PollutedAreas** to track the progress of environmental cleanup.

- **PollutedArea**: Targeted by a **CleanupAction** for pollution reduction.
- **CleanupAction**: The effort to clean up or mitigate the pollution in a specific **PollutedArea**.

---

## 8. **User** ↔ **Achievement**  
Users earn **Achievements** based on their actions, such as participating in projects, completing cleanups, or reporting pollution. **Achievements** are linked to users and serve as a reward or recognition for contributions.

- **User**: Receives **Achievements** for their activities (e.g., cleaning a certain number of areas or participating in a project).
- **Achievement**: A recognition or reward system for **Users** based on their contributions.

---

## 9. **User** ↔ **Notification**  
Users can receive notifications for various platform activities, including updates about their own actions, new **PollutedAreas**, or **Projects** they are involved in. Notifications are a direct form of engagement with the platform.

- **User**: Receives notifications about environmental updates or actions relevant to them.
- **Notification**: Alerts and information sent to **Users** based on their preferences and activities.

---

## 11. **User** ↔ **Complaint**  
Users can submit **Complaints** about unauthorized pollution or environmental issues to the relevant authorities through the platform. These complaints are tracked, and users can receive updates on their status.

- **User**: Files a **Complaint** regarding pollution or environmental issues.
- **Complaint**: Represents the formal complaint submitted by a **User** regarding pollution.

### Summary of Relationships:
- **Users** are central to the platform and interact with various entities, such as **Projects**, **PollutedAreas**, **CleanupActions**, and **Achievements**.
- **Projects** and **PollutedAreas** are closely linked, as projects aim to mitigate pollution in specific areas.
- **PollutionMeasurements** provide the data that informs users and authorities about the state of pollution.
- **Notifications** help keep users informed about changes and new actions regarding **PollutedAreas**, **CleanupActions**, and more.

These interactions create a dynamic, user-driven system where volunteers, organizations, and citizens can work together to address pollution and improve the environment.
