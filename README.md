# **TravelGroupVerynice by TehOLimauAis**
![logo](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/logo.png)
![logo_long](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/logo_long.png)


**Team:** Ethan Law, Ng Jun Han, Kong Shiun Soon, Oh Yu Pin

**Problem Statement:** Travel Planner

**Video Presentation:** https://youtu.be/0-g9pGYspjQ

**Presentation Slides:** https://docs.google.com/presentation/d/13nh8TMh9HmR3a1JJKax5czCiJ2gYp4GQV1cdGrkzcUs/edit?usp=sharing

**Prototype** https://officialtgv.netlify.app/

## **1\. Project Overview**

**The Problem:**

Travelling in large groups is cost saving via cost-splitting and group discounts. However, according to a survey from the United States, 46% of people prefer to travel in small groups (\<7) while only 8% of people prefer to travel in large groups (\>20).

Our research shows that lack of flexibility, decision paralysis, budget mismatches and lack of leaders are the main factors that cause this disparity despite the many benefits that large group travelling can bring. 

The main stakeholders involved in travel planning are the travellers themselves. This group is highly segmented with many different types of groups such as leisure vacationers, families and corporate clients. The platform has no revenue without their demand. Other stakeholders include the inventory suppliers such as airlines and railways, lodging providers, ground transportation and local tour operators. Government and regulatory bodies are stakeholders as they enforce consumer protections laws, aviation regulations, data privacy standards and taxation policies for the companies involved. 

One of the main apps that exist in the market is [trip.com](http://trip.com) which is an online travel agency that has a website and mobile app which allows users to book flights, hotels, trains, rental cars, tours, attraction tickets and much more services related to travel. [Trip.com](http://Trip.com), despite its whole package coverage of all travelling essentials, is not recommended for travelling in large groups due to the fact that their systems are not made for it. For example, flight and hotel search engines generally cap a single transaction to 8 or 9 passengers and large groups are forced to divide into multiple, disconnected bookings. Another major issue is variable pricing, when a large group is split across multiple transactions, the algorithm will treat them independently. Thus, the first group might lock in a cheap fare while the remaining members get hit with dynamic price increases for the exact same flight, negating the savings that a large group might receive. Additionally, [trip.com](http://trip.com) displays the public retail rates and cannot negotiate any specialised group contracts for big groups. 

**Our Solution:**

Our web app will be similar to [trip.com](http://trip.com) but with added features catered to large group travel. The app will include unique and special features such as a branching itinerary, Tinder-based matching for group formation, activity and location recommendations based on member preferences, live positional updates on maps for all group members, attendance tracking and midpoint location or activity suggestions and a midpoint suggestion where users are recommended locations and attractions that they can add for their itinerary. The web app will still include features that are found in common travel planners such as the travel page for flights, hotel searching and booking and more.

Feature Set: 

* General Features  
  * Flight details  
  * Weather forecasting  
  * Peak and low season indicator  
  * Location/Activities  
  * Google Reviews and relevant information of locations  
  * Hotel Searching & Booking  
  * Map  
  * Trip Travel Page  
* Unique Features  
  * Branching itinerary  
  * Tinder-based matching for group formation  
  * Activity and location recommendation based on member preferences  
  * Live positional update of all group members  
  * Attendance tracking  
  * Midpoint location/activity suggestion

## **2\. Ideation & Process**

### **2.1 Ideas We Considered**

Table of every distinct idea generated, with why each was kept or dropped, order it so that chosen ideas are listed first

| Idea                                            | Why it was dropped / kept |
| :----                                           | :----                     |
| TravelGroupVerynice TGV (Chosen)                | <ul><li>Niche (some features targeted towards large travel groups)</li><li>Everyone can use the app (wide audience)</li><li>Came up with multiple unique ideas to distinguish our idea from existing solutions</li></ul> |
| StudyLah (Dropped)                              | <ul><li>Does not really match the problem statement</li><li>Focus on study plan only instead of other things students may be also tackling (assignments, jobs, etc)</li><li>The digital twin idea is heavily reliant in user discipline and requires additional effort to operate, which we think will cause more harm than good.</li></ul>  |
| Dedicated AI Stress Organizer DAISO (Dropped)   | <ul><li>Exactly following the problem statement, can only stand out if our solution is better than all the other competitors</li><li>Accuracy concerns with rPPG biosignature readings depending on using native app or PWA</li></ul> |

### **2.2 Ideation Boards**
#### **2.2.1 Lifestyle Track: Beating the Burnout (Idea 1)**

**DAISO**

Utilize existing stress-related datasets to develop a continuously improving product based on dataset context and product impact. Conventional, simple problems that do not require data are already being solved by web apps and programmers. Data enables us to tackle more complex problems with uncertain assumptions that would otherwise be difficult or impossible to validate without empirical evidence.
Ideas proposed here are noble. Only research codes and papers but not commercialized products. We are making these products marketable with a human touch of UI UX and business model.

**TILES**
The TILES dataset combines physiological (heart rate, breathing rate, ECG), behavioral (steps, sleep, smartphone usage), environmental (temperature, humidity, light, motion), proximity/location (RSSI), participant metadata, and survey (stress, fatigue, well-being, job satisfaction) data, making it useful for machine-learning analysis and prediction of workplace stress, fatigue, well-being, and job performance.

Product example:
**HRFriend**. Uses data from employee medical records, and install tracker on smartphone and smartwatch to gague employee stress at work. Company can allocate mental health resources to stressed employees to improve productivity and to make your company have halo effect


**StudentLife**
The StudentLife dataset includes columns such as school, sex, age, studytime, failures, absences, internet, G1, G2, and G3, and can be used to analyze and predict how students’ demographics, study habits, attendance, and academic history influence their final academic performance.

Product example:
**STUFriend**. Uses data from student school records, gague student performance at school. School can allocate mental health resources to retarding students to improve productivity and to make your school have halo effect.



**WESAD**
WESAD (Wearable Stress and Affect Detection) is a multimodal physiological dataset containing ECG, EDA, EMG, respiration (Resp), temperature (Temp), 3-axis acceleration (ACC_X, ACC_Y, ACC_Z), BVP, and stress/affect labels, which can be used to develop and benchmark stress and emotion detection models, with potential for translating these signals into smartphone- or smartwatch-derived proxies for real-world stress monitoring.

Product example:
**SigmaLimiter**. For those who are always locked in (workaholics). Uses phone camera / webcam + screentime to derive biomechanics data and current task data, classify it as a stress inducing behavior or not, and determine if it is healthy for the user to continue and recommend breaks.

**DAIC-WOZ**
DAIC-WOZ is a multimodal depression-detection dataset containing participant-level columns such as Participant_ID, Gender, PHQ8_Score, PHQ8_Binary, and individual PHQ-8 symptom scores, along with time-aligned transcript (start_time, stop_time, speaker, value), audio, and facial features, making it suitable for developing and evaluating AI models for depression detection and severity prediction.

Product example
**HelpTherapy**. Therapy is suggestive and sometimes invasive. This product will interview you like a therapist (with LLM) but listens to you like therapists will (Audio and image processing) and gives you a more accurate diagnosis. 
(or can rebrand as a tool to help therapists to read microexpressions or people who cant afford therapy.)


 

TILES, StudentLife and WESAD core concept is similar to an existing product called https://sumondo.co/, where the change is just the business model and accessibility. Changing a business model or another way to do the same thing with accuracy drawbacks for more accessibility is not an absolute and noble  improvement over an existing solution, but rather a considerable alternative.
For DAIC-WOZ, these ideas already exist.
Wysa already provides AI-based mental-health conversations.
Woebot Health also uses AI to provide mental-health support.
CU Medicine's multimodal depression app already combines facial expressions, voice, language, and other data to assess depression.
Conclusion: HelpTherapy is not very unique in its current form. Its strongest way to stand out would be to help therapists by analyzing these signals and highlighting potential concerns, rather than trying to replace therapists or diagnose patients itself.



DAISO (Dedicated AI Stress Organizer) - A connection of scheduling, activity classification, analysis and convenient stress measurements based on bio signatures. Supercharged with forecasting / action call and self-experimental discovery framework for new interventions.

For every scheduled activity from external calendar sources, it can be automatically or manually classified as a stress type activity or recovery typed activity with subcategories. Biosignatures are taken before and after said activity with a mobile device and an increase / decrease in stress level is recorded. At the end of a period (a week or a month), a summary of the data is shown to the user with suggestions based on the data.

The collected data can also be used to predict stress levels, allowing the application to notify users when their upcoming schedule may be too demanding and suggest adjustments.

Once data is sufficient, the application is able to aid the user by providing an experimentation framework for the users self discovery by scheduling new recovery methods while collecting data for a future comparison.

The app will also remind the user for constant recalibration to adapt to changes in baseline of the users


Research process
1. **Can PRV detect stress?**
Yes. Studies using PPG-based devices report high accuracy — one model hit 94.3% accuracy classifying 5 levels of mental stress (source), and another hit ~95% for stress and ~98% for depression (source).
WESAD, a widely-used benchmark dataset (chest + wrist sensors, 15 subjects, lab-induced stress via public speaking/math tasks), also shows PRV features can separate stress from baseline/amusement, typically in the 80–95% range
Caveat: PRV tracks HRV well at rest, but that agreement gets worse under stress or movement — exactly when you're trying to measure it (source).
2. **Fingertip camera PPG vs. wearables for resting PRV**
Fingertip camera PPG is very accurate at rest — correlation with ECG of r=.997 (source).
It can even beat wrist wearables: fingertip HRV error stayed at 0.15ms regardless of conditions, while wrist PPG error jumped up to 12x if contact pressure wasn't perfect (source).
Independent long-term testing backs this up for daily resting HRV tracking (source).
3. **Is facial camera PPG a good fallback for resting PRV?**
For heart rate alone — yes, nearly as good as fingertip (r=.997) (source).
For PRV/HRV specifically — much weaker. One study found HR correlation of 0.86 but HRV correlation of only 0.25–0.33 (source). Facial PPG is also very sensitive to motion and lighting, with errors up to 30+ BPM in handheld/real-world conditions (source).
Simple ranking (most to least reliable for resting PRV): chest strap/wearable ≈ fingertip camera PPG > wrist wearable (poor fit) > facial camera PPG.

#### **2.2.2 Lifestyle Track: Beating the Burnout (Idea 2)**


**StudyLah**

```
1. The StudyLah Concept
StudyLah is a social learning-planning platform for university students. Creators publish structured study blueprints that describe a learning strategy, required effort, sequence, milestones and suitable context. Followers can copy a blueprint, but StudyLah does not reproduce its timetable blindly. It adapts the method to the follower’s real availability and observed learning behaviour.



1.1 Problem Statement
Students are surrounded by advice but still struggle to convert it into a realistic routine. A timetable copied from a high-performing student may demand different hours, energy patterns, course intensity or personal responsibilities. Static templates preserve someone else’s schedule; ordinary planners organise tasks the student already knows how to create; generic schedule generators often lack evidence about where the routine came from and whether it worked for comparable learners.
1.2 Specific Target Group
The initial target group is Malaysian university students managing classes, assessments and independent study, particularly students who feel overloaded, lack a reliable study routine or repeatedly abandon ambitious schedules. This directly fits CodeNection’s Lifestyle and Personal Productivity direction and its burnout-related problem context.
```

#### **2.2.3 Lifestyle Track: Planning an Escape**

#### **TGV**
![Affinity](https://i.imgur.com/MO29KDG.png)
![tgv_ideation1](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/tgv_ideation1.png)
![tgv_ideation2](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/tgv_ideation2.png)

### **2.3 Mentor Consultation**

| Date | Mentor | Feedback Received | What Was Changed |
| :---- | :---- | :---- | :---- |
| 2 Sept | Teng Wei Herr | <ul><li>For frontend, use Next.js or React, whichever framework that AI is proficient at</li><li>Develop an app that the creator themselves would use</li></ul> | Finalize on Next.js as one of the frontend frameworks |
| 2 Sept | Khor Jia Quan | <ul><li>Suggested we go for the travel planner idea as it is more broad and can cover everyone, not just for students only with the stress tracker</li></ul> | More confidence in travel planner idea |
| 3 Sept | Varsha Selvakumar | <ul><li>Travel Planner (Kong):</li><ul><li>Midpoint recommendation for reconvening, weather and crowd factor prediction (is niche and good)</li></ul></ul><ul><li>StudyLah (Ethan):</li><ul><li>Refine prediction model, copy study plan is good idea, use prediction model to suggest new template quiz to match users to new templates</li><li>NEED PREDICT BECAUSE STOP BURNOUT</li><li>behavior analysis</li></ul></ul><ul><li>Stress Tracker (JunHan):</li><ul><li>Combine Ethan and JunHan idea</li><li>Feature is good, but less niche since it is 1 to 1 to what problem statement wants</li><li>More competition since everyone solving same problem</li><li>This idea will compete in who solves the problem better (JunHan idea), rather than who solves a better problem (Kong idea)</li></ul></ul><ul><li>Idea Tips:</li><ul><li>Find the problem and find features to solve it</li><li>See if can map a feature to a problem statement</li><li>find niche \-\> smaller audience, better space user \-\> problem \-\> feature</li></ul></ul> | More confidence in travel planner idea, add midpoint recommendation, weather & crowd prediction into idea. |
| 4 Sept | Iris Yan | <ul><li>Pitch for JunHan idea was good and attention grabbing</li><li>Pitch for travel planner has intended customer base zoned in (good and niche)</li><li>Introduce Tinder-based grouping system to group people in large travel groups</li></ul> | Finalize on travel planner idea, add Tinder-based grouping system to idea. |

## **3\. Design & Prototype**

**UI Prototype:** https://officialtgv.netlify.app

![planner](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/planner.png)
![subgroups](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/subgroups.png)
![suggestions](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/suggestions.png)
![newact](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/newact.png)
![companion](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/companion.png)
![commu](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/commu.png)

## **4\. What Makes It Different**

Our travel planner solution is more niche, as in the selling point features are more targeted towards large travel groups. The following features are what makes our solution unique.

### Branching Itinerary

Unlike the majority of existing travel planners on the market which uses a linear itinerary system, in which everyone has to participate in the same activity, our solution introduces a branching itinerary system, similar to a “Choose Your Own Adventure” system, where members of a travel group can decide on which branch/activity they want to partake in based on their personal preferences. With this system, there is no longer a need to follow a linear itinerary in which some of the activities may not be interesting to some group members.

Based on the activities that the users have chosen in the main itinerary page (branching itinerary), a personal itinerary will be visible in their own app, in which there will be a linear itinerary that shows the activity that they will be partaking in. This helps to alleviate the visibility and clarity concerns that a complicated branching itinerary may bring forth.

### Tinder-Based Matching for Group Formation

This feature is specially catered towards large travel groups, such as company and class trips, where everyone may not be familiar with each other, not to mention everyone having different and varied preferences. For large group trips, it is expected that people will form groups with other members that they are familiar with. Instead of everyone forming their own small groups based on friends, our solution introduces a group matching system that is based on the preferences of the members, and this is especially useful for getting to know other like minded individuals in the group as well as making new friends.

The way this feature works is that, members in the group trip can create subgroups with specific preferences in mind. For example, member A creates a subgroup with the preference “extreme sports”, and member B creates a subgroup with the preference “shopping”. If member C wants to join a subgroup and their preference is more towards shopping, they will be recommended the subgroup that was created by member B first. If they are interested, they can swipe right to join the group, or swipe left to dismiss the group and see the next best recommendation based on their preferences. If none of the groups suit the member, the member can choose to create their own subgroup in which other people can join in. 

This feature complements the Branching Itinerary system, as in there can be completely differing activities for the given timeframe. Groups that are more interested in shopping can go shopping, while groups that are more interested in extreme sports can partake in extreme sports. There is no longer a need to worry about finding an activity that caters to everyone with this grouping system and branching itinerary system.

### Activity/Location Recommendations Based on Group Member Preferences

When users first create an account, they will be prompted to fill in their personal preferences (or aggregate tags), as in what kind of activities they prefer partaking in. For example, a user can select “sightseeing”, “slow-walks”, and “animals” as their preferences. Upon joining a travel group, their preferences will be taken into consideration, along with all the other group members by the recommendation engine. The recommendation engine will provide a group fit score for the recommended activity based on the aggregate tags of everyone on the trip, and it will also provide a reason for why that specific activity was recommended.

### Midpoint Location/Activity Suggestion

As an extension to the recommendation engine, our solution also provides a midpoint location/activity suggestion for when multiple groups/branches need to reconvene. Our app will propose potential candidates that are ranked on spread and calculate the imbalances between all groups/branches, and it is not just based on the total distance that has to be traveled.

### Trip Companion (Branch Location Tracking on Map and Attendance Tracking)

The Trip Companion is a tab/page in the app that displays the user’s personal itinerary (the activities/branches that they have chosen) with live “DONE, NOW, NEXT” states. Other than that, it also displays the locations of all other branches to easily track where the entire group is. Furthermore, there is also an attendance tracking feature where the attendance for the branch can be viewed by the members partaking in that branch. Based on the member’s location to the branch location, it will automatically mark that member as “arrived”, and it can be viewed by the other members in the same group.

## **5\. Technical Architecture & Feasibility**

We have chosen the PWA approach over native applications mainly because we want to avoid unnecessarily long development times, and our solution will still be solid without pure native support.

---

The frameworks and technologies used for each component are as follows:


CLIENT

- Next.js (App Router) \+ TypeScript — Frontend framework for building the web app with server/client rendering and type-safe JavaScript.

- TanStack Query — Fetches, caches, synchronizes, and updates server/API data on the client.

- Zustand — Lightweight global state management for UI and application state.

- Yjs (client-side CRDT) — Enables real-time collaborative editing by synchronizing state between users/devices.

- SVG \+ d3-shape — Creates interactive vector graphics, charts, paths, and custom visualizations.

- Radix UI / shadcn \+ Tailwind — Provides accessible UI components and utility-based styling for building the interface.

- Serwist (service worker / PWA) — Adds offline support, caching, background functionality, and installable PWA capabilities. (Optional)

NATIVE WRAPPER

- Capacitor — Wraps the web application as native iOS and Android apps and provides access to native APIs.

- Capacitor Push Notifications plugin — Integrates native push notifications on iOS and Android.

- Capacitor Background Geolocation — Tracks device location in the background for location-based functionality.

- Capacitor Share / Calendar plugins — Provides native sharing and calendar integration.

- App Store / Play Store distribution — Packages and distributes the application through Apple App Store and Google Play Store. (Optional)

APPLICATION LAYER (Python)

- FastAPI — High-performance Python framework for building REST APIs and backend services.

- Strawberry GraphQL — Creates a type-safe GraphQL API using Python type hints. (Optional)

- Pydantic v2 — Validates, parses, and serializes API request/response data.

- Uvicorn \+ Gunicorn — Runs and manages Python application processes in production.

- Clerk / Supabase Auth — Handles authentication, user identity, sessions, and access control.

REAL-TIME & JOBS (Python)

- FastAPI WebSockets — Provides persistent real-time connections between clients and the backend.

- pycrdt / pycrdt-websocket — Provides Python-side CRDT synchronization for collaborative real-time features.

- Celery \+ Redis (broker) — Runs background and asynchronous jobs such as notifications and data processing.

- firebase-admin (FCM v1) — Sends push notifications to Android and iOS devices through Firebase Cloud Messaging.

DATA LAYER (Python)

- SQLAlchemy 2.0 (async) \+ asyncpg — Provides asynchronous database access and ORM functionality for PostgreSQL.

- GeoAlchemy2 (PostGIS) — Adds geographic functionality such as coordinates, distances, and spatial queries.

- pgvector-python — Enables storing and searching AI/vector embeddings in PostgreSQL. (Optional)

- redis-py (async) — Provides asynchronous Python access to Redis for caching, queues, sessions, and real-time data.

- boto3 (S3 / Cloudflare R2) — Manages file uploads, downloads, and object storage.

- Alembic — Handles database schema migrations as the application evolves.

EXTERNAL SERVICES

- Mapbox / Google Maps Platform — Provides maps, geocoding, routing, places, and location services. (pay as you go, technically free)

- Tomorrow.io (weather) — Provides real-time weather data and forecasts. [free](https://support.tomorrow.io/hc/en-us/articles/31227543026708-How-to-Use-the-Tomorrow-io-API)

- BestTime.app (crowd forecasting) — Predicts how busy or crowded locations are at different times. [provides limited free credits](https://besttime.app/)

- Klook / GetYourGuide / Viator / Booking.com (Agoda) — Provides travel activities, tours, attractions, hotels, and booking inventory. (no mentions of pricing, called Demand API on [Booking.com](http://Booking.com)) (have to apply for Klook but its free, might even earn commissions, can be B2B or affiliate)

- Open Exchange Rates (FX) — Provides foreign-exchange rates and currency conversion data. (json file when making API call)

- Resend / Postmark (email) — Sends transactional emails such as verification, notifications, and receipts. (postmark API is free, 500 messages per call, 50MB payload size)

INFRA & HOSTING

- Vercel (Next.js hosting) — Hosts and deploys the Next.js frontend with CDN and automated deployments.

- Fly.io / Railway / AWS Fargate (Python API \+ WebSocket) — Hosts backend APIs, workers, and persistent WebSocket services.

- Cloudflare (CDN) — Provides global caching, DNS, security, CDN delivery, and edge networking.

TOOLING / DEVOPS

- uv or Poetry — Manages Python dependencies, virtual environments, and project configuration.

- GraphQL Codegen — Generates TypeScript types and client code from the GraphQL schema. (Optional)

- pytest \+ Playwright — Tests the Python backend and performs end-to-end browser testing. (Optional)

- GitHub Actions — Automates CI/CD workflows such as testing, building, and deployment. (Optional)

- Sentry \+ Datadog/Grafana — Monitors errors, performance, logs, metrics, and infrastructure health. (Optional)

DATABASES / STORES

- PostgreSQL — Primary relational database for users, trips, bookings, and application data.

- PostGIS — PostgreSQL extension for storing and querying geographic/spatial data.

- pgvector — PostgreSQL extension for storing and searching vector embeddings. (Optional)

- Redis — In-memory data store for caching, queues, sessions, rate limiting, and real-time coordination. 

- S3 / Cloudflare R2 — Object storage for images, documents, uploads, and other large files.

![arch](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/arch.png)

The plan to build the application will be like so:  
![build](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/build.png)


We will be building this in a serial manner, with a frontend and backend split during the development stage once the core components are done. Testing and QA will be done after integration, and we will only proceed to deployment if the testing results are satisfactory.
