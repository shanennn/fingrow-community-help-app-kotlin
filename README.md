<img width="366" height="796" alt="image" src="https://github.com/user-attachments/assets/cb337267-df62-4bea-bd80-eb45b155859b" /># FinGrow

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
<img width="366" height="796" alt="image" src="https://github.com/user-attachments/assets/ab8c5343-84a6-4a08-9382-1a15bdc5d420" />
Community Share: browse, search and filter donated items. Each item shows how many units are left, or "Reserved" when none remain.

<img width="366" height="796" alt="image" src="https://github.com/user-attachments/assets/a250f587-e55f-4fa3-925b-d56aa060545b" />
**Item Details (Reserver View):** A person who reserved the item sees the same details, plus a "Your reservation was accepted!" message once the donor approves. Unreserve Item cancels the reservation and returns the unit to the pool.

<img width="366" height="796" alt="image" src="https://github.com/user-attachments/assets/38fe951f-4568-47bf-8e74-257e16562548" />
**Item Details (Owner View):** The donor sees the item photo, how many units are left (12 of 16), the description and pickup location on a map. Edit Post and Delete Post manage the listing, and View Reservations shows how many units have been claimed (4 of 16).
