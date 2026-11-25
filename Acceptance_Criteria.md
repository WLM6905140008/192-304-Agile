# Acceptance Criteria — GTG (Global Transportation Guide)

| Course | 192-304 Agile Software Development |
| Project | GTG — Global Transportation Guide |
| Name & ID | Wai Lwin Moe (6905140008)

## 1. Purpose

These acceptance criteria explain how the team will decide whether the GTG MVP features are complete and working correctly. The team should test each criterion before accepting the feature.

## 2. Feature Acceptance Criteria

### AC-01 — Open the GTG website

- [ ] Given a user opens the website, when the home page loads, then the GTG name and city selection options are visible.
- [ ] The home page does not show a broken layout or an error message during normal use.

### AC-02 — Select a city

- [ ] Given a user is on the home page, when the user selects Bangkok, Tokyo, or Singapore, then the website opens the correct city page.
- [ ] The selected city name is clearly displayed.
- [ ] The user can return to the home page or city selection.

### AC-03 — View transport options

- [ ] Given a user opens a supported city page, when the page is displayed, then the transport overview shows the available metro/train, bus, and taxi information stored for that city.
- [ ] Each transport type has a clear name and a short explanation or relevant information.
- [ ] A transport type with no available data is not presented as though complete information exists.

### AC-04 — Select a starting place and destination

- [ ] Given a user is viewing a city page, when the user opens the route selection controls, then the user can choose from the supported starting places and destinations in that city.
- [ ] The available place choices belong to the selected city.
- [ ] The same place cannot be selected as both the starting place and destination unless the team has a clear reason to support that journey.

### AC-05 — View a matching route

- [ ] Given a supported starting place and destination have route data, when the user searches for the route, then the website displays at least one matching route.
- [ ] Each result identifies the transport type and gives a short route description.
- [ ] Given no route is stored for the selected places, when the user searches, then the website displays a clear message such as **No route information is available for this selection yet.**

### AC-06 — View estimated price and travel time

- [ ] Given a route result is displayed, when the user views its details, then an estimated price or price range is shown with the correct city currency.
- [ ] The minimum estimated price is not higher than the maximum estimated price.
- [ ] An estimated travel time is shown in minutes or hours and minutes.
- [ ] The page clearly identifies the price and travel time as estimates.

### AC-07 — View ticket and payment information

- [ ] Given ticket or payment information is available for a route, when the user opens the route details, then the accepted payment methods are displayed.
- [ ] Where ticket-purchase information is available, the page explains where the user can buy a ticket.
- [ ] If payment or ticket information has not been verified or is unavailable, the page says that the information is unavailable or does not display an unsupported claim.

### AC-08 — Read step-by-step instructions

- [ ] Given a route has instructions, when the user opens its details, then the instructions are displayed as numbered steps in the correct order.
- [ ] Each step uses simple English and identifies important stations, stops, or actions when the data is available.
- [ ] The instructions are readable on a mobile phone screen.

### AC-09 — Use the website on different screen sizes

- [ ] Given a user opens the website on a mobile phone, when the user views the main pages and route details, then important content and controls fit the screen and can be used without horizontal scrolling.
- [ ] Given a user opens the website on a desktop screen, when the user views the same pages, then the layout remains clear and usable.
- [ ] Text, buttons, and form controls are readable and not overlapping.

### AC-10 — Navigate between pages

- [ ] Given a user is viewing route details, when the user chooses the back or city navigation option, then the correct previous page or city page is displayed.
- [ ] The user does not need to restart the website to select another route or city.

## 3. Overall Definition of Done

The MVP can be accepted when all of the following are true:

- [ ] The three MVP cities — Bangkok, Tokyo, and Singapore — are available for selection.
- [ ] The main functional requirements marked **Must have** in the Requirements Specification have been implemented.
- [ ] The acceptance criteria above have been tested on the available test data.
- [ ] No critical defect prevents users from selecting a city or viewing route information.
- [ ] The main user flow works on mobile and desktop screen sizes.
- [ ] Estimated prices and travel times are labelled clearly.
- [ ] The team has checked the sources for the published transportation information.
- [ ] The four project documents are saved in the repository's `docs` folder.
- [ ] The GitHub repository is public and contains the latest project documentation.

## 4. Suggested Test Data

The team should add real, checked routes to the database before using them for final acceptance testing. The following are examples of test cases; they are not claims that these routes, prices, or times have already been entered or verified.

| Test case | Input | Expected result |
|---|---|---|
| TC-01 | Select Bangkok | Bangkok city page opens |
| TC-02 | Select Tokyo | Tokyo city page opens |
| TC-03 | Select Singapore | Singapore city page opens |
| TC-04 | Search for a route that exists in the database | Matching route details are displayed |
| TC-05 | Search for a route that does not exist in the database | A clear no-route message is displayed |
| TC-06 | Open a route with fare and time data | Estimated fare, currency, and travel time are displayed |
| TC-07 | Open a route with payment data | Available payment and ticket information is displayed |
| TC-08 | Open a route on a mobile screen | Instructions and controls remain readable and usable |
