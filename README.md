# WellLoad by Provexant

### *Tan Kher Er, Chong Jing Yung, Chu Gin Nie, Wong Xin Yu*

### Problem Statement: Stress & Workload Manager

### Video Presentation: https://youtu.be/KMuQsJPIs6M

### Presentation Slides: https://www.canva.com/design/DAHU7_vkeEw/rLJ86yP6g_No9VoIDJ-eqA/edit


## 1. Project Overview

***

### The Problem

Students have information about their lives scattered across different apps, but no simple way to understand their overall capacity.  They often experience burnout from academic deadlines, extracurricular activities, and personal responsibilities. Many existing wellness and productivity apps require users to manually enter tasks, habits, and mood data, which creates more effort for already-stressed students.

Apps such as Forest and Pomodoro tools mainly focus on productivity or focus time. They may not give students a clear view of their overall capacity across physical, mental, social, and time-related demands. They also often feel complex to use.

Students need a simple way to understand their stress and capacity without repeatedly filling in forms or switching between many different apps. 

***

### Our Solution

WellLoad is a low-friction student capacity-management app that combines information from the tools students already use and turns it into one simple view of their current capacity. WellLoad connects to existing services such as Calendar, Apple Health, Strava, Sleep, and location-based services.

The app turns this data into a simple 5-vector capacity view across:

- **Mental** — mental workload and stress
- **Time** — schedule and time commitments
- **Physical** — exercise, movement, and physical activity
- **Social** — social activities and commitments
- **Life Admin** — everyday responsibilities and personal tasks

WellLoad provides a simple overall picture of how much capacity the user is using and when they may need to recover. 

***

### What Makes WellLoad Different

WellLoad's main differentiator is connectivity and automatic logging. Instead of trying to replace every app a student already uses, WellLoad acts as an aggregator that brings relevant information together.

1. **AI Quick Logging**

Users can enter a simple sentence such as: "I played badminton for one hour." AI identifies the activity, duration, and relevant category, then creates the activity log.

2. **Camera-to-Log**

Users can take a photo of their current activity. For example, a photo of a badminton court or study desk can be analyzed by AI to identify the activity and create a log.

3. **Snap-to-Log Reminders**

If users frequently forget to track their activities, WellLoad can send occasional reminders asking them to quickly capture what they are doing. The reminder can be customized or disabled according to the user's preference. The goal is to make tracking feel like a quick interaction rather than another task to complete.

***

<u>**Phase 1 — Connectivity, Data & Visualisation**</u>

1. **Connected Data Engine** - collects relevant information from services that users already use.

Potential data sources include:

- Calendar events
- Apple Health
- Strava
- Steps
- Sleep
- Physical activity
- Location data

This reduces manual data entry and allows WellLoad to build a more complete picture of the user's daily activities.

2. **5-Area Capacity Visualiser** -  converts the collected information into five areas:

Mental | Time | Physical | Social | Life Admin

The dashboard gives users a quick overview of where their current capacity is being used. Users can see their overall situation in one place, rather than looking at individual data points from different applications

3. **AI Quick Logging** - users can manually add activities by typing a short description.

For example: "Studied in the library for three hours."

AI extracts relevant information such as:

- Activity
- Duration
- Category

The user can then confirm or edit the generated entry before saving it.

4.  **Camera-to-Log** - provides another low-effort way to record activities.

Users take a photo of what they are currently doing, and AI analyzes the image to identify a possible activity. For example: Photo → Badminton activity detected → User confirms → Activity logged


<u>**Phase 2 — Stress Detection & Recovery**</u>

1. **Capacity & Stress Detection**

WellLoad continuously evaluates available signals to identify when the user's workload or stress level is becoming too high. When the user's capacity reaches a predefined threshold, WellLoad moves from tracking to intervention. The purpose is not simply to tell users: "You are stressed." Instead, WellLoad provides a practical next step.

2. **Recharge Pick**

When WellLoad detects potential overload, it generates a Recharge Pick based on the user's interests and current context. For example:

- User enjoys walking → Suggest a nearby walking route
- User enjoys singing → Suggest karaoke
- User enjoys quiet environments → Suggest a library or quiet space
- User enjoys art → Suggest a nearby gallery
- User needs physical recovery → Suggest a short, low-intensity activity

3. The prototype can use the Google Places API to retrieve relevant nearby locations and provide users with an actionable recovery option. 


<u>**Phase 3 — Motivation & Social Support** </u>

1. **Recovery Zoo** - a secondary motivation feature.

Users earn points by completing recovery actions and maintaining healthy recovery habits. These points can be used to customise a digital chicken mascot with:

- Accessories
- Outfits
- Other cosmetic items

The mascot represents the user's recovery consistency, making the process more engaging without turning WellLoad into a traditional gamified productivity app.

2. **Healthy Social Accountability**

Users can optionally connect with friends and view each other's recovery progress. The purpose is to encourage healthy accountability, rather than competition based on productivity. For example, friends can encourage each other to:

- Take recovery breaks
- Maintain healthy routines
- Complete recovery activities
- Stay consistent

***

## 2. Ideation & Process 

### 2.1 Ideas We Considered

| Idea | Why it was dropped / kept |
|---|---|
| **A — Connected Data + 5-Area Capacity Dashboard (Chosen)** | **Kept.** This directly addresses the problem of students having their workload, health, and activities scattered across different apps. By connecting existing data and presenting it across Mental, Time, Physical, Social, and Life Admin, users can understand their overall capacity without manually tracking everything. |
| **B — AI Quick Logging + Camera-to-Log (Chosen)** | **Kept.** Manual tracking was identified as one of the main barriers to existing wellness apps. AI Quick Logging and Camera-to-Log reduce the number of steps needed to record an activity, supporting our goal of making WellLoad as effortless as possible. |
| **C — Recharge Pick + Location-Based Recommendations (Chosen)** | **Kept.** Instead of only showing users that their capacity is high, WellLoad provides an immediate and personalized action they can take. Combining user interests with location allows the recommendation to become practical and actionable. |
| **D — Recovery Zoo + Social Accountability (Chosen)** | **Kept as a secondary feature.** Gamification and social accountability can encourage users to maintain healthy recovery habits. However, these features are not the core solution, so they are positioned as motivation layers rather than the main functionality of WellLoad. |
| **E — Insights Analysis** | **Dropped.** We considered adding more detailed insights and analytics based on the user's data. However, this mainly adds information rather than solving the user's need to take action. Since our goal is a minimalist and easy-to-use experience, we chose to prioritize actionable recommendations instead. |
| **F — Combining Multiple Existing Wellness Features** | **Dropped.** We considered combining common features from existing productivity and wellness apps into one platform. However, this approach was not sufficiently innovative and would still require users to interact with multiple features step by step. It did not address our core problem of reducing user effort. |
| **G — Extensive Manual Tracking** | **Dropped.** Requiring users to manually enter tasks, moods, habits, and activities would create additional work for students who are already experiencing stress. This directly conflicts with our low-friction design principle. |
| **H — Productivity Tools** | **Dropped.** Features such as Pomodoro timers and focus sessions were considered, but they focus primarily on productivity rather than understanding the user's overall capacity and preventing overload. Existing tools already address this area effectively, so it was not a strong differentiator for WellLoad. |

***

###  Ideation Boards

<img width="1448" height="616" alt="image" src="https://github.com/user-attachments/assets/2d5dd54d-76f1-4ed8-b060-dc60a665e777" />

**Row 1**: We started with a smarter task list. Dropped it because a better list still encourages users to take on more and this behaviour causes burnout.

**Row 2**: We considered detailed self-reporting. Simplified because students won’t journal every activity. The Log feature became one-tap entry or Camera-to-Log.

**Row 3**: We initially considered a focus timer. Dropped it because it optimises study time while ignoring sleep, social activities, and other responsibilities. This led to the 5-Area Capacity view instead.

***

**User Flow:**

<img width="638" height="794" alt="image" src="https://github.com/user-attachments/assets/11970d6b-f6f9-4752-b5d4-765b7859ca50" />

**Stage 1 Set Up**

User enters Classes & Deadlines → WellLoad automatically adds them to Time & Life Admin.

**Stage 2 Check Capacity**

User opens Home → Views their 5 Areas and current daily capacity.

**Stage 3 Take Action**

If capacity is high → WellLoad shows What to Do Next → User receives one recovery recommendation or finds a relaxing spot nearby.

**Stage 4 Recover & Track**

User completes the recovery activity → Earns progress in My Zoo → Pet improves as the user maintains healthy recovery habits.

***

**Problem Tree**

<img width="1364" height="816" alt="image" src="https://github.com/user-attachments/assets/0eb9ebca-1796-44df-a048-424d5fb0e4a4" />


**Problem:** Students manage classes, workouts, club duties, and personal commitments across different apps, making their total workload and remaining capacity difficult to see.

**Key Insight:** The core problem is invisible overload. Students often realise they have exceeded their capacity only after it affects their grades, health, or engagement. So, we focus on measuring capacity rather than treating the effects.

**Solution:** WellLoad brings these commitments into one view and uses a 5-Area Capacity Score to show how much capacity students have left. Rest is also included, encouraging balance rather than simply doing more.

**Limitation:** WellLoad cannot remove social pressure to say yes, but making capacity visible gives students a clearer basis for setting boundaries, with future ideas such as decline scripts and shareable capacity views.

***

### 2.3 Mentor Consultation 

<table>
  <thead>
    <tr>
      <th>Date</th>
      <th>Mentor</th>
      <th>Feedback Received</th>
      <th>What Was Changed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td rowspan="5"><strong>10 September</strong></td>
      <td rowspan="5"><strong>Zach Khong</strong></td>
      <td>The mascot and social comparison made the app feel like “Forest but competitive with friends.” They should not be the main focus.</td>
      <td>Repositioned Recovery Zoo and friend comparison as secondary motivation features rather than the core product.</td>
    </tr>
    <tr>
      <td>The strongest and most unique idea is connectivity between existing apps such as Calendar, Strava, and Apple Health.</td>
      <td>Made the Connected Data Engine a core feature and positioned WellLoad around connected capacity management.</td>
    </tr>
    <tr>
      <td>Users should not have to fill in many forms or manually log every activity.</td>
      <td>Added AI Quick Logging and Camera-to-Log to reduce manual input.</td>
    </tr>
    <tr>
      <td>A BeReal-style notification could make activity logging more natural and effortless.</td>
      <td>Added Snap-to-Log reminders that prompt users to capture their current activity for AI to log.</td>
    </tr>
    <tr>
      <td>The prototype has too many screens, making it harder for judges to understand within a short time.</td>
      <td>Simplified the prototype to focus on Connectivity → 5-Area Capacity → AI Logging → Recovery Recommendations.</td>
    </tr>
  </tbody>
</table>

***

## 3. Design & Prototype 

UI Prototype: https://canva.link/13ofm66bpa6b781 

## 4. What Makes It Different 

| **Feature**                     | **What Makes It Different**                                                                                                                                           |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **5-Area Capacity Visualiser**  | Combines Mental, Time, Physical, Social, and Life Admin into one capacity view, helping students see their overall load instead of tracking separate tasks or habits. |
| **Connected Data Engine**       | Aggregates data from existing apps such as Calendar, Apple Health, and Strava, reducing the need for users to manually track everything.                              |
| **AI Quick Logging**            | Users describe an activity in one short sentence, and AI automatically identifies the activity, duration, and category instead of requiring form-based tracking.      |
| **Camera-to-Log / Snap-to-Log** | Uses a quick photo to identify and log activities. BeReal-style reminders make tracking more natural and less like completing another task.                           |
| **Recharge Pick**               | Instead of only telling users that their capacity is high, WellLoad provides one actionable recovery suggestion based on their interests and current context.         |
| **Location-Aware Recovery**     | Combines user interests with nearby locations to turn a generic wellness suggestion into a specific place or activity the user can actually do.                       |
| **Recovery as Progress**        | The Recovery Zoo makes rest and recovery visible through rewards, shifting the mindset from “doing more” to “recovering better.”                                      |

## 5. Technical Architecture & Feasibility 

<img width="2678" height="1498" alt="image" src="https://github.com/user-attachments/assets/94f9323c-42e9-40fd-9ba9-c3fbc957e0e7" />

### Frontend

| **Technology**             | **Purpose**                                                                                                                                         |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| **React Native with Expo** | Builds a cross-platform mobile application. Expo provides access to native features such as location, notifications, camera, and calendar services. |
| **Tamagui**                | Provides reusable UI components and styling for the mobile application.                                                                             |
| **Zustand**                | Manages client-side application state.                                                                                                              |
| **TanStack Query**         | Handles server-state fetching, synchronization, and caching efficiently.                                                                            |

### Backend

| **Technology**               | **Purpose**                                                         |
| ---------------------------- | ------------------------------------------------------------------- |
| **Supabase Auth**            | Handles user authentication and account management.                 |
| **Supabase Edge Functions**  | Executes secure backend logic and external API calls.               |
| **Supabase Storage**         | Stores user-generated files and media.                              |
| **Row-Level Security (RLS)** | Protects user data by controlling access at the database row level. |

### Database

| **Technology**          | **Purpose**                                                                       |
| ----------------------- | --------------------------------------------------------------------------------- |
| **Supabase PostgreSQL** | Stores relational application data and supports efficient querying and analytics. |

### AI API

| **Technology**                          | **Purpose**                                                                          |
| --------------------------------------- | ------------------------------------------------------------------------------------ |
| **OpenAI Responses API (GPT-5.6 Luna)** | Generates personalized recovery suggestions based on user context and capacity data. |

### External APIs and Native Services

| **Technology / API**   | **Purpose**                                                                      |
| ---------------------- | -------------------------------------------------------------------------------- |
| **Google Places API**  | Provides nearby place information for location-aware recovery recommendations.   |
| **Expo Location**      | Accesses the user's location for context-aware features.                         |
| **Expo Calendar**      | Connects with calendar data to understand users' schedules and time commitments. |
| **Expo Notifications** | Sends reminders and Snap-to-Log notifications.                                   |
| **Apple HealthKit**    | Accesses health and activity data to support physical capacity tracking.         |

### Hosting & Application Development

| **Technology**                      | **Purpose**                                                                                   |
| ----------------------------------- | --------------------------------------------------------------------------------------------- |
| **Expo Application Services (EAS)** | Builds and distributes iOS application versions.                                              |
| **Supabase Cloud**                  | Hosts the database, authentication services, storage, and backend functions.                  |
| **GitHub**                          | Provides version control and supports collaborative development.                              |
| **Supabase Secrets**                | Securely stores API keys and other sensitive environment variables used by backend functions. |

***
