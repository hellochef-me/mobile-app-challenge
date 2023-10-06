# Hello Chef - Mobile App Assignment

## Brief

Your assignment is to create an event discovery web app using Ticketmaster Discovery API.
Link: https://developer.ticketmaster.com/products-and-docs/apis/discovery-api/v2/

Your app should consist of two screens and it should ideally be powered by Vue.js (v2 or v3, any will do).

Feel free to add tests how you see fit.

## Features

### Home Page

1. This page is used to search / discover events. It offers the following inputs:
    - **Country:** A drop-down of available countries that the user can choose from. You can find the list under the "Supported Country Codes" section on Ticketmaster's developer portal.
    - **Search Term:** Search for an event by its name / venue name / genre name, etc.
    - **Start Date:** (optional) Filter with a start date after this date (format e.g. 2021-12-20T17:05:00Z)
    - **End Date:** (optional) Filter with a start date before this date (format e.g. 2021-12-31T17:05:00Z)
2. Once the user enters all the fields and hits the **Search** button, she is shown a list of all the events available for the chosen country and matching the given search term.
3. This list can be further filtered, sorted, and paginated as per the following points:
4. List filters:
    - **includeTBA** boolean flag - yes, to include with date to be announce (TBA)
    - **includeTBD** boolean flag - yes, to include with a date to be defined (TBD)
5. List sorters:
    - Name (ascending & descending)
    - Date (ascending & descending)
    - Relevance (ascending & descending)
6. List pagination:
    - A size drop-down with appropriate options e.g. 10, 20, 50, 100, 200
    - Page number selections

### Event Details Page

1. This page shows details of any event as identified by its `id`.
2. The following details need to be displayed on this page:
    - Name
    - Venue
    - Information
    - Images
    - Date & time
    - Classification (segment, genre)
    - Price
3. You may display any additional details you'd like using the API response.

## UI

Feel free to use any CSS framework of your choice and create the UI as per your liking. (Bonus points for making it mobile first & responsive.)

## API

1. You can aquire an `apikey` by registering on the https://developer.ticketmaster.com/ portal.
2. You'll find that the `Event Search` API endpoint is ideal for finding events using `keyword` and `country` parameters. You can also filter your search results by date (`startDateTime` and `endDateTime`) and other parameters available in the documentation. You may use `page` & `size` parameters to implement pagination. Sorting is also available using the `sort` keyword.
3. The `Get Event Details` API endpoint is suitable to render the **event details** page.


## Submission & Presentation

1. Please create a public GitHub / BitBucket repository for your project.
2. Your repository must have a detailed `README.md` with instructions on how to set up & run your code locally.
3. It must not contain the words “hellochef” or “challenge”.
4. We would like you to present your work no later than 7 days from the day you receive your assignment.
5. Accordingly, please send us the link to your repository at least 1 day prior to the presentation meeting for a review.
6. The presentation would be done in these steps:
    - Run your code locally
    - Give us a UI and features walkthrough
    - Explain your code
    - Run tests, if any

---

> Have questions? We would love to answer. Mail us at techchallenge@hellochef.me
