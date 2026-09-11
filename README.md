# **TravelGroupVerynice by TehOLimauAis**
![logo](https://raw.githubusercontent.com/4isherman/TGV/refs/heads/main/assets/logo.png)


**Team:** Ethan Law, Ng Jun Han, Kong Shiun Soon, Oh Yu Pin

**Problem Statement:** Travel Planner

**Video Presentation:** https://youtu.be/0-g9pGYspjQ

**Presentation Slides:** https://docs.google.com/presentation/d/13nh8TMh9HmR3a1JJKax5czCiJ2gYp4GQV1cdGrkzcUs/edit?usp=sharing

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

| Idea | Why it was dropped / kept |
| :---- | :---- |
| TravelGroupVerynice TGV (Chosen) | Niche (some features targeted towards large travel groups) Everyone can use the app (wide audience) Came up with multiple unique ideas to distinguish our idea from existing solutions |
| StudyLah (Dropped) |  |
| Dedicated AI Stress Organizer DAISO (Dropped) |  |

### **2.2 Ideation Boards**

![Affinity](https://i.imgur.com/MO29KDG.png)

### **2.3 Mentor Consultation**

| Date | Mentor | Feedback Received | What Was Changed |
| :---- | :---- | :---- | :---- |
| 2 Sept | Teng Wei Herr | For frontend, use [Next.js](http://Next.js) or React, whichever framework that AI is proficient at.  Develop an app that the creator themselves would use. | Finalize on [Next.js](http://Next.js) as one of the frontend frameworks |
| 2 Sept | Khor Jia Quan | Suggested we go for the travel planner idea as it is more broad and can cover everyone, not just for students only with the stress tracker. | More confidence in travel planner idea |
| 3 Sept | Varsha Selvakumar | Travel Planner (Kong): Midpoint recommendation for reconvening, weather and crowd factor prediction (is niche and good) StudyLah (Ethan): Refine prediction model, copy study plan is good idea, use prediction model to suggest new template quiz to match users to new templates NEED PREDICT BECAUSE STOP BURNOUT behavior analysis Stress Tracker (JunHan): Combine Ethan and JunHan idea. Feature is good, but less niche since it is 1 to 1 to what problem statement wants. More competition since everyone solving same problem. This idea will compete in who solves the problem better (JunHan idea), rather than who solves a better problem (Kong idea) Idea Tips: Find the problem and find features to solve it. See if can map a feature to a problem statement  find niche \-\> smaller audience, better space user \-\> problem \-\> feature | More confidence in travel planner idea, add midpoint recommendation, weather & crowd prediction into idea. |
| 4 Sept | Iris Yan | Pitch for JunHan idea was good and attention grabbing.  Pitch for travel planner has intended customer base zoned in (good and niche). Introduce Tinder-based grouping system to group people in large travel groups | Finalize on travel planner idea, add Tinder-based grouping system to idea. |

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
