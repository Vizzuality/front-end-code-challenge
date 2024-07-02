# Front-end-code-challenge

First thing first. This coding challenge is about creating a space for you to share with us how you work and reason, what things you care about when doing coding work, and how you approach problem solving. As such, through this challenge we are not expecting to check if you know the finest algorithms, have all the right answers to a given situation or if you are the best coder in the world. We believe there are no right or wrong answers, so please make yourself comfortable and focus on what you know best.

You will be tasked with creating a React SPA showing bicycle networks around the world on a map.

**Please submit your ideas to us within two weeks (max).** This will give us enough time to review your challenge with the rest of the team before the next interview. During this interview, we will take some time to explore your coding challenge submission together and ask any clarifying questions we might have.

The challenge is designed so that a candidate can **complete it within 8 to 10 hours**. If something comes up and you can't deliver within the two-week time-frame, let us know. We are flexible.

## Design

You can find the design of the application here:

- [Interactive prototype](https://www.figma.com/proto/0MNqMneHvxahQZ6pknjzlq/Frontend-Challenge?page-id=1166%3A4310&node-id=5110-10913&viewport=4865%2C-2607%2C0.79&t=UlhDbVzZT1c5dezR-1&scaling=scale-down&content-scaling=fixed&starting-point-node-id=5110%3A10913)
- [UI kit](https://www.figma.com/design/0MNqMneHvxahQZ6pknjzlq/Frontend-Challenge?node-id=1166-4310)

## Technical requirements

### Technologies

For this challenge, you will use the following technologies and libraries:

- [Next.js](https://nextjs.org/) with the App router.
- [Typescript](https://www.typescriptlang.org/).
- [Tailwind CSS](https://tailwindcss.com/).
- [Shadcn/ui](https://ui.shadcn.com/).

You will build a React application using the technologies and design listed above. It will comply with the following requirements:

### README

Your submission should also include a README file where you can document your work, describe the features and the architectural decisions that you made. Feel free to share your thoughts about the challenges that you faced implementing your code.

### Data

The bicycle network data is fetched from the following API: https://api.citybik.es/v2/

The country data is provided in the `data` folder in this repository.

### Deployment

In order to access the application, we are asking you to **create a repository** (on GitHub for example) and to **deploy the application** using a cloud platform of your choice (we recommend [Vercel](https://vercel.com/)). Don't forget to share the links to both the repository and public application URL.

### App structure

#### Main view

There is a list of all the bicycle networks and for each of them:

- Name.
- Location (city and country).
- Companies operating the network (can be multiple).
- Link to access the detail view.
- There is a map showing all the bicycle networks.
- Clicking on a network opens the detail view.
- There is a country filter that affects both the list and the map:
  - Only one country can be selected at once.
  - The selected option is stored in the URL (e.g. `?country=FR`).
  - When reloading the page, the filter is still applied.
- There is a search input that affects both the list and the map:
  - The search is performed against the name of the networks and name of the operating companies.
  - The keyword is stored in the URL (e.g. `?search=velib`).
  - When reloading the page, the filter is still applied.
- BONUS: There is a way to centre and zoom the map around the user's location
- BONUS: The list of networks is paginated

#### Detail view

- The detail view **must be accessible by URL**.
- There is general information about the bicycle network:
  - Name.
  - Name of the companies operating the network (can be multiple).
  - Location (city and country).
- There is a list of all the bicycle stations belonging to the network:
  - Name.
  - Number of free bikes.
  - Number of empty slots.
- There is a button to go back to the main view. 
- There is a map showing all the bicycle stations.
- Clicking on a station on the map opens a tooltip:
  - Name.
  - Number of free bikes.
  - Number of empty slots.
- BONUS: The list of bicycle stations is paginated
- BONUS: The list of bicycle stations can be sorted by free bikes and empty slots (ascending and descending).

If any of these requirements are unclear, feel free to reach out for guidance. If this challenge proves to be too much work, it's better to focus your attention on fewer items.

## What we'll look for

Once you've handed the challenge to us, we'll look for the following:

- Type safety is applied.
- How data is managed (fetching, parsing...).
- State management.
- Navigation and URL handling.
- Styling, attention to detail.
- Performance optimization and accessibility.

These points (and more) will be discussed with you in a follow-up technical meeting.

## What's next?

Once you submit your solution, our developers will review your code challenge, taking your experience level into account. The sample code provided by you should be in a state considered as a "production" ready - where each requested element is prepared and potentially ready to review with your colleagues.

Here are a few hints that can help to align your code with the requirements:

- Does the application realize all the required features?
- Is anything missing from the specification?
- Is the code clear, maintainable, and easy to understand for other developers? Is it extendable?
- Does the readme file describes all the features and covers all the information that is essential for the project?
- Don't focus only on the "happy path" - have you covered all the edge cases that you faced?

Good luck!

**"The Challenge" has been created with the sole intention of being used as a guiding document for the current recruitment process. This means we won't be using it (all or parts of it) within our projects.**
