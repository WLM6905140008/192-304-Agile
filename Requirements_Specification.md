# Requirements Specification — GTG (Global Transportation Guide)

| Course | 192-304 Agile Software Development |
| Project | GTG — Global Transportation Guide |
| Name & ID | Wai Lwin Moe (6905140008)

## 1. Introduction

### 1.1 Purpose

This document describes the requirements for the GTG website MVP. It explains what the website should do and the basic quality requirements it should meet. It will guide the team's design, development, and testing.

### 1.2 Project Description

GTG is a mobile-friendly website for travelers who need transportation information in unfamiliar cities. The first version will cover Bangkok, Tokyo, and Singapore. It will show transport options, basic routes, estimated prices, estimated travel times, ticket/payment information, and simple instructions in English.

### 1.3 Intended Users

- Tourists visiting a city for the first time.
- International students who are unfamiliar with local transportation.
- First-time travelers who need clear and simple travel information.

## 2. User Problem and Needs

The team's interviews with 10 people identified common problems: users may not know which type of transport to take, how to find the correct route or station, how much a journey costs, or which payment methods are accepted. Different transport systems and local-language signs can also be confusing. Users need clear route details and useful information in one place.

Therefore, GTG should make basic transportation information easy to find and understand.

## 3. Product Scope

### 3.1 Included in the MVP

- City selection for Bangkok, Tokyo, and Singapore.
- Transport overview for metro/train, bus, and taxi.
- Basic routes between selected popular places.
- Estimated price or price range and currency.
- Estimated travel time.
- Ticket and payment information, including where to buy tickets when known.
- Step-by-step instructions in simple English.
- Responsive pages for mobile and desktop screens.

### 3.2 Not Included in the MVP

- Live vehicle locations, arrival times, traffic, or service alerts.
- GPS navigation or automatic route tracking.
- Online ticket sales or payment processing.
- User registration or personal accounts.
- Complete travel planning for accommodation, restaurants, or attractions.
- Automatic multi-language translation.
- Full route coverage for every location in each city.

## 4. Functional Requirements

Functional requirements describe the actions and information that the website must provide.

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | The website shall display the GTG name and a clear way to select a city. | Must have |
| FR-02 | The website shall provide Bangkok, Tokyo, and Singapore as the initial city choices. | Must have |
| FR-03 | After a user selects a city, the website shall display basic information about that city. | Must have |
| FR-04 | The city page shall show the transport types available in the project data: metro/train, bus, and taxi. | Must have |
| FR-05 | The user shall be able to select a starting place and a destination from the supported places in the selected city. | Must have |
| FR-06 | The website shall display matching route information when a route is available for the selected places. | Must have |
| FR-07 | Each route shall show its transport type and a short route description. | Must have |
| FR-08 | Each route shall show an estimated price or price range and the correct currency. | Must have |
| FR-09 | Each route shall show an estimated travel time. | Must have |
| FR-10 | Route details shall show relevant ticket and payment information, including accepted payment methods and where to buy tickets when known. | Must have |
| FR-11 | Route details shall show simple, numbered steps explaining how to follow the route. | Must have |
| FR-12 | When no route is available for a selected pair of places, the website shall show a clear message instead of an empty or broken result area. | Must have |
| FR-13 | The website shall provide a clear way for the user to return to the city selection or city information page. | Should have |

## 5. Non-Functional Requirements

Non-functional requirements describe how well the website should work.

| ID | Requirement | Priority |
|---|---|---|
| NFR-01 Usability | Text and instructions shall use simple English and clear labels that are easy for first-time travelers to understand. | Must have |
| NFR-02 Responsive design | Main pages and features shall be usable on common mobile phone, tablet, and desktop screen sizes. | Must have |
| NFR-03 Readability | Text shall have a readable size and sufficient contrast against the background. | Must have |
| NFR-04 Consistency | City, route, price, travel-time, and payment information shall use a consistent layout across the three cities. | Should have |
| NFR-05 Performance | Main pages should load within a reasonable time on a normal internet connection. | Should have |
| NFR-06 Reliability | The website shall handle missing route results or missing optional information with a clear message and without crashing. | Must have |
| NFR-07 Data accuracy | Route, fare, travel-time, and payment information shall be checked against reliable sources before it is published. | Must have |
| NFR-08 Data clarity | Estimated fares and travel times shall be clearly labelled as estimates. | Must have |
| NFR-09 Maintainability | City, place, route, and payment information shall be stored in an organized structure so that the team can update it. | Should have |

## 6. Main User Flow

1. The user opens the GTG website.
2. The user selects Bangkok, Tokyo, or Singapore.
3. The website displays the selected city's transport overview.
4. The user selects a starting place and destination from the available places.
5. The website displays the matching route or a message that no route is currently available.
6. The user opens a route and reads its transport type, estimated price, estimated time, ticket/payment information, and step-by-step instructions.
7. The user can return to the city page or select another city.

## 7. Business Rules and Data Rules

1. The MVP supports only Bangkok, Tokyo, and Singapore.
2. A route's starting place and destination must belong to the same city as the route.
3. Estimated minimum price must not be greater than estimated maximum price.
4. Estimated travel time must be greater than zero minutes.
5. Route instructions must be displayed in the correct order.
6. A route must be connected to one transport type, such as metro/train, bus, or taxi.
7. Prices must show the currency used in the relevant city.
8. Missing information must be shown as unavailable or omitted clearly. The website must not invent ticket or payment details.
9. Prices and travel times are estimates and may change. GTG does not guarantee the final fare or journey duration.

## 8. External Interfaces and Data

### 8.1 User Interface

The website should use clear navigation, readable text, simple labels, and a consistent layout. The main user actions are selecting a city, selecting a route's starting place and destination, and reading route details.

### 8.2 Data Sources

The team should collect route, fare, travel-time, and ticket information from reliable sources, such as official transport operator websites and official city travel information pages. The team should record the source and last-checked date for route information where possible.

### 8.3 Internet Connection

Users need an internet connection to open the website. The MVP does not require live transport data or GPS access.

## 9. Limitations and Assumptions

- The route and transport information is prepared by the team and is not updated automatically in real time.
- Only selected popular places and routes will be included in the first version.
- English is the MVP language.
- Price and time estimates may differ from the user's actual journey.
- The exact number of routes per city will depend on the information the team can verify and enter during development.

## 10. Requirement Change Process

A team member who suggests a change should explain the reason and how it affects the MVP. The team should review the change together. Changes that are not necessary for the MVP should be added to a future-work list rather than delaying the agreed main features.
