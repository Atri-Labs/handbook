# Welcome to the Atri Handbook! ✨

The goal of this repository is to share a deeper dive into what we are building, the thought process behind the decisions we have made along the way and where we are headed. 

<img src="assets/theatre.jpeg" alt="drawing" width="1000"/>

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Welcome to the Atri Handbook! ✨](#welcome-to-the-atri-handbook-)
  - [Product](#product)
    - [What are we building at Atri Labs?](#what-are-we-building-at-atri-labs)
    - [Can the frontend and backend development be decoupled?](#can-the-frontend-and-backend-development-be-decoupled)
    - [Development experience](#development-experience)
      - [Contextualizing development experience](#contextualizing-development-experience)
    - [Extensibility of Atri editor](#extensibility-of-atri-editor)
      - [What type of extensibility is allowed at the moment?](#what-type-of-extensibility-is-allowed-at-the-moment)
    - [The project's dependency graph shows that some NodeJS and Express-related libraries. What does that mean?](#the-projects-dependency-graph-shows-that-some-nodejs-and-express-related-libraries-what-does-that-mean)
  - [Traction](#traction)
    - [Downloads](#downloads)
    - [Companies](#companies)
    - [All community stats](#all-community-stats)
  - [Open-source community](#open-source-community)
    - [Nuanced perspective on contributions](#nuanced-perspective-on-contributions)
    - [How to understand our contributor base?](#how-to-understand-our-contributor-base)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Product
### What are we building at Atri Labs?

- We are building a full-stack framework on top of React (think in the leagues of Next.js, Remix.run, Gatsby.js, etc.)
- Since it is a full-stack framework, users can build both frontend and backend. 
- To build frontend, they can a mix of React code and productivity tools such as visual editor.
  - Hence, depending on their web development skills, project-specific requirements and preferences, they can write as much or as little code as they want.
- The backend can be written in Python. 
  - We are planning to add support for NodeJS soon.
- Once the app is built, it can be then be deployed to GitHub pages, AWS, etc. in one step using our command line tool. 

> ⚠️ Atri framework is not a low-code/no-code tool. It is a developer-focused product that is **bringing the best of the no-code world into the pro-code world**. 

### Can the frontend and backend development be decoupled?

Since Atri framework is a full-stack framework, by definition, it provides the complete ecosystem to build frontend and backend together. However, some web development projects may not need a backend. 

There are two different types of web development projects and Atri framework supports development of both of them. 

1. **Static pages**
   - Static content does not change based on user or her interaction with the content (e.g. "About company" page). 
   - Hence, it does not need a backend.

2. **Dynamic pages**
   - Dynamic content is either personalized for each user (e.g. order history) or dependent on user interaction (e.g. form submission). 
   - In either case, we need to build its backend.

   2.1. **JAMStack**
   - It is a special way of handling backend development work where you outsource almost all of it to services and write minimal backend code.

### Development experience

1. The framework is evoked through the `Terminal` from inside the project repository.
2. The software runs locally on the user's system during the development period. 
3. The user events are compiled at each `Build and Run`. This generates the corresponding code and automatically saves it in the project repository.

> 💻 **Code is always available to the user**

4. Besides, Atri developers do not need to write REST APIs.  Instead, they rely upon the Atri object model which acts as a single source of truth. 
   - Frontend and backend teams now do not need to spend time in maintaining documentation for their APIs 
   - This also has other benefits such as reducing compliance breaches because it is not possible to accidentally send sensitive information from backend to frontend without modifying the object model. 

> 🤯 **No REST APIs**

#### Contextualizing development experience 

To contextualize this development experience, we can think of how web developers build a React app using the `create-react-app` library. 
- The library abstracts away many of the commonly required, cumbersome tasks (both easy and hard problems).
- At the same time, developers still retain complete access and control of their code. 

### Extensibility of Atri editor

Extensibility has been a very important guiding principle from Day 1 of the development of Atri editor. 

> 💡 **We are planning to explore opportunities to file software patents for our unique implementations of extensibility.**

#### What type of extensibility is allowed at the moment?

At the moment, users can extend the editor by adding new components. 

Offering our community to extend the Atri editor in other ways is not our focus for the next 6-8 months. Our two key engineering and business goals are:

- Release stable version (1.0.0) of Atri framework
- Build a community of 100k+ users of Atri framework 

Our view is that the right time to seek community contributions on the extensibility of Atri editor (and Atri framework, as well for that matter) will be when we would have achieved project-community fit.  

### The project's dependency graph shows that some NodeJS and Express-related libraries. What does that mean?



## Traction

### Downloads

One can track the daily downloads of our project [here](https://pepy.tech/project/atri).

<a href="https://pepy.tech/badge/atri" target="_blank"><img src="https://pepy.tech/badge/atri" alt="Downloads"></a>

### Companies

We are compiling a list of companies where our users work.  

### All community stats

We are preparing a data room that will give a holistic view of our community activity across platforms. 
- This is itself an open-source project that can be used by other open-source companies. 

## Open-source community

### Nuanced perspective on contributions

Some industry outsiders have this perception that `contributions = code contributors shown in GitHub` and consequently `fewer contributions = bad`. 

This is incorrect in several respects because:

1. This ignores the role that support infrastructure plays in the success of an open-source project. 
   - This support infrastructure includes documentation, utility libraries, community management, etc. 
   - None of this appears on the `GitHub code contributions` graph. 
   - As a result, more and more projects are moving towards the [all-contributors](https://allcontributors.org/) specification because it acknowledges and highlights all types of contributions. 
 
2. Not every project wants external contributions to its codebase. In our case, we have been operating at a rapid iteration mode. 
   - To seek active code contributor base would mean that we will have an additional overhead of maintaining rigorous documentation of our codebase. (Note that this is different from the documentation that we maintain for Atri app creators). 
   - Moreover, in order to make meaningful contributions to our framework, one needs to possess intermediate to advanced proficiency in web technologies. Sourcing such engineers would require considerable effort from our end. Hence, it does not land high on our priority list. 

3. To handle inbound interest to contribute, there are fewer issues that we could assign to a newcomer. 

   -  is not most people's cup of tea. 
   - a casual open-source contributor may contribute meaningfully to a library's repository but will not be suitable 

>❓While analyzing the health of an open-source project, one needs to take a nuanced look into which metrics matter for an open-source project at a particular stage. 

### How to understand our contributor base?

>❗ Make sure you have read [the above section](#nuanced-perspective-on-contributions) to develop a more nuanced understanding on how a maintainer thinks about code contributions during the earlier stages of an open-source project.

- Code contributors is not a correct metric to gauge the health of our community. 
- One should instead look at our [downloads](#downloads) and all-contributors-count instead. 

<a href="https://pepy.tech/badge/atri" target="_blank"><img src="https://pepy.tech/badge/atri" alt="Downloads"></a> [![All Contributors](https://img.shields.io/badge/all_contributors-52-orange.svg?style=flat-square)](#contributors-)