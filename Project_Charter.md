# Project Charter — GTG (Global Transportation Guide)

| Project name | GTG — Global Transportation Guide |
| Course | 192-304 Agile Software Development |
| Project type | Group project / Minimum Viable Product (MVP) |
| Name & ID | Wai Lwin Moe (6905140008)

## 1. Project Background

Travelers can find it difficult to use public transportation in a city or country they have never visited. Transportation systems, routes, ticket prices, and payment methods are different in each place. Travelers may also have difficulty understanding local signs or knowing which station and vehicle to use.

To understand these problems, the team interviewed 10 people about their experiences with transportation in unfamiliar places. The interviews showed that people want clear route information, estimated prices and travel times, ticket and payment details, and simple instructions. They also prefer to find this information in one place instead of searching several websites or applications.

GTG (Global Transportation Guide) will be a mobile-friendly website that collects basic transportation information for selected cities. The first version will cover Bangkok, Tokyo, and Singapore.

## 2. Project Purpose

The purpose of GTG is to help tourists, international students, and first-time travelers understand local transportation more easily. The website will provide practical information in simple English so users can make a more informed choice about how to travel between popular places.

## 3. Project Objectives

The project aims to:

1. Provide a simple way to select Bangkok, Tokyo, or Singapore.
2. Show an overview of the main transportation options in each city, including metro/train, bus, and taxi.
3. Provide basic route guides between selected popular places, such as airports, city centers, and attractions.
4. Show estimated travel prices and travel times for each available route.
5. Explain ticket options, accepted payment methods, and where users can buy tickets.
6. Give clear, step-by-step instructions in plain English.
7. Make the website usable on both mobile phones and desktop screens.

## 4. Target Users and Stakeholders

**Main target users**

- Tourists visiting a city for the first time.
- International students who are new to a city or country.
- First-time travelers who need help understanding local transportation.

**Other stakeholders**

- The three student team members.
- The course instructor, who reviews the project and its documentation.
- People who provide feedback during user testing.

## 5. Project Scope

### In scope for the MVP

- A home page with a city selection feature.
- Initial city information for Bangkok, Tokyo, and Singapore.
- A transport overview for metro/train, bus, and taxi in each selected city.
- A basic route guide using a prepared list of popular starting points and destinations.
- Estimated fare or fare range and estimated travel time for each route.
- Ticket and payment information, including where to buy tickets when this information is available.
- Simple step-by-step route instructions in English.
- A responsive, mobile-friendly layout.

### Out of scope for the MVP

- Live GPS tracking or turn-by-turn navigation.
- Real-time arrival times, delays, traffic, or service alerts.
- Purchasing tickets or making payments through GTG.
- User accounts, profiles, and saved trips.
- A complete trip planner for hotels, restaurants, or activities.
- Automatic translation into multiple languages.
- Coverage of every city or every transportation route.

These features may be considered for a later version, but they are not required for the first release.

## 6. Main Deliverables

1. A mobile-friendly GTG website containing the agreed MVP features.
2. Transportation and route information for Bangkok, Tokyo, and Singapore.
3. Project documentation in the repository's `docs` folder:
   - Project Charter
   - Requirements Specification
   - Acceptance Criteria
   - Database Design
4. Basic testing of the MVP features and correction of important defects found during testing.
5. A publicly accessible GitHub repository containing the project files and documentation.

## 7. Success Criteria

The MVP will be considered successful when:

- Users can select and open each of the three planned cities.
- Each city page shows the available metro/train, bus, and taxi information recorded by the team.
- Users can choose a supported starting place and destination and view at least one matching route when route data exists.
- Each displayed route includes an estimated price, currency, and travel time.
- Route details show relevant ticket/payment information and numbered instructions when those details are available.
- The main pages can be used on common mobile and desktop screen sizes without important content being cut off.
- The team has tested the main user flows and documented known limitations.

## 8. Project Approach

The team will use an Agile approach and develop the MVP in small steps. The team can review progress, divide tasks, test completed features, and update the backlog when needed. The team should check that the website still meets the agreed requirements after changes are made.

## 9. Assumptions and Constraints

**Assumptions**

- The first version will present information in English.
- The team will collect and enter route and transport information before users access it.
- Prices and travel times will be estimates, not guaranteed live values.
- The MVP will use a limited selection of popular places and routes in each city.
- Users will have an internet connection to access the website.

**Constraints**

- The project must be completed within the time and resources available for the course.
- The MVP has a limited number of cities and routes.
- Transportation prices, payment rules, and services may change, so information needs to be checked and updated by the team.
- The project should use tools and technologies that the team can support during the course.

## 10. Main Risks and Responses

| Risk | Possible effect | Response |
|---|---|---|
| Route, fare, or payment information is incorrect or out of date | Users may follow confusing instructions or misunderstand costs | Use reliable sources, record when information was last checked, and show that prices and times are estimates |
| Too much information is added for the first release | The team may not finish the MVP on time | Prioritize the three cities and a small set of popular routes |
| Instructions are too complicated | Users may still feel confused | Use short sentences, numbered steps, and clear place names |
| Website layout does not work well on phones | Main target users may have difficulty using the website | Test the main pages at mobile and desktop sizes |
| Team tasks are not clearly divided | Work may be delayed or duplicated | Agree on task owners and review progress regularly |