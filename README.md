An Android app where people in a community can share donations and job opportunities.
Built as a group project for AMIT3353 Mobile Application Development (Diploma in Computer Science, TAR UMT).

## Features
- Register, log in, forgot password, and set a new password
- Profile page and edit profile
- Donation posts: browse a list, filter, view details, and see who reserved an item
- Job posts: browse a list, filter, view details, and see applicants
- Create posts with input validation
- Photos for posts (camera support)
- Your own activity list

## Tech stack
- Kotlin, Jetpack Compose, Material 3
- Navigation Compose, ViewModel
- Supabase (authentication, database, storage)
- Ktor, kotlinx.serialization

## How to run
1. Open the project in Android Studio.
2. Wait for Gradle sync to finish.
3. Run on an emulator or a phone (Android 8.1 or higher).

## My part
I was responsible for the **Community Share** module of the FinGrow app, which allows users to browse, search and reserve donated items shared by the community.

- Donation list screen with search and category filtering
- Item details screen
- Reserve function, where the donor can accept or reject each person who wants to reserve the item
- Dedicated filter screen to narrow results by category and state
- Quantity system: a donor specifies how many units of an item they are giving away, and other users can reserve a specific amount based on the remaining quantity. The post automatically becomes unavailable once all units are reserved.

## Team
Group project with three coursemates.

## Screenshots
<img width="250" alt="image" src="https://github.com/user-attachments/assets/807c46c1-4f4b-417f-a3d0-b1a781cd7ba2" />

Community Share: browse, search and filter donated items. Each item shows how many units are left, or "Reserved" when none remain.

<img width="250" alt="image" src="https://github.com/user-attachments/assets/c36e5019-e4c1-49bb-a294-3d47022c4b09" />

**Item Details (Reserver View):** A person who reserved the item sees the same details, plus a "Your reservation was accepted!" message once the donor approves. Unreserve Item cancels the reservation and returns the unit to the pool.

<img width="250" alt="image" src="https://github.com/user-attachments/assets/4ecf5fdf-e613-47ee-81c8-9c1f2f0af742" />

**Item Details (Owner View):** The donor sees the item photo, how many units are left (12 of 16), the description and pickup location on a map. Edit Post and Delete Post manage the listing, and View Reservations shows how many units have been claimed (4 of 16).
