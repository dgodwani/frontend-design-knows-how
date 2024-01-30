# frontend-design-knows-how


<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="logo.jpg" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Frontend Design Knows How</h3>

  <p align="center">
    A comprehensive document covering the know hows of frontend system design 
    <br />
   <p>Show your support by giving a ⭐&nbsp;&nbsp;to this repo</p>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#grooming">Grooming</a></li>
    <li><a href="#solutioning">Solutioning</a></li>
    <li>
      <a href="#design">Design</a>
      <ul>
        <li><a href="#hld">HLD</a></li>
        <li><a href="#lld">LLD</a></li>
        <li><a href="#guidelines">Design Document Guidelines</a></li>
      </ul>
    </li>
    <li><a href="#technology-choice">Technology Choice</a></li>
    <li><a href="#ui-frameworks-and-libraries">UI Frameworks & Libraries</a></li>
    <li><a href="#api-handling-and-communication protocols">API handling and communication Protocols</a></li>
  </ol>
</details>


<!-- Introduction -->
## Introduction

Welcome to the comprehensive guide on Frontend System Design. This document is your go-to resource for understanding the various stages of frontend design and implementing best practices to ensure the successful creation and long-term maintainability of web application components. Whether you are a seasoned developer or just starting, this guide aims to equip you with the knowledge needed for both new component development and maintaining a structured frontend system.

Document Overview:
- Explore the different stages of frontend system design, from conceptualization to deployment. 🚀
- Acquire insights into the significance of each design stage for creating a robust and scalable architecture. 🔍
- Delve into guidelines and best practices to inform decisions for enhanced performance, user experience, and maintainability. 🛠️
- Refer to a high-level process overview figure for a quick understanding of the frontend system design journey. 🌐
- Connect frontend system design to the product life cycle for a broader context of product development. 🔄

<!-- Grooming -->
## Grooming
Grooming is a crucial step in the project life cycle, focusing on refining requirements and addressing potential issues in the early planning stages. Identifying and resolving issues at this phase is significantly more efficient than dealing with them after the code has been written, allowing developers to create a solid design for their software.


### In the Grooming Stage:
During the grooming stage, the team, consisting of engineers, designers and product stakeholders, engages in detailed discussions to refine the requirements of the product. This includes exploring use cases, understanding use case realizations, and further scoping the project.


Questions to ask at this stage:
- Does the design align with the product vision and goals? 🎯
- Is the proposed requirements technically feasible? 💻
- Can requirements be broken down following the MoSCoW rule? 📦
- How can MoSCoW rule define the Minimum Viable Product? 🚀
- What scale and performance levels are expected? ⚖️
- Who is the target audience, and how does the frontend cater to their preferences and needs?
- What are the dependencies and constraints to address? 🤝
- What are the accessibility and usability requirements for the frontend?
- Are there any technical constraints or limitations that could impact the design?
- Are there specific design considerations or patterns that should be applied to meet the product's objectives?
- Will the application be used on mobile devices?
- Is it B2B/B2C/Internal/Consumer Facing etc.


What to Do in This Stage:

- Collaboratively gather requirements.
- Thoroughly scope the project.
- Prioritize backlog items.
- Detail requirements for clarity.
- Clarify Ambiguities, Address and resolve uncertainties.

Outcome: 

The outcome of the grooming stage is a fine set of requirements, both short term and long term for a component. These can further be split at a high-level as:

- Functional requirements
- Non Functional requirements
- Failover requirements
- Operational requirements
- Functional dependencies

Reference: https://www.aha.io/roadmapping/guide/release-management/what-is-a-product-backlog

## Solutioning
Solutioning is a pivotal phase in the project life cycle, where the focus shifts from refined requirements to crafting a comprehensive plan for implementation. It involves assembling various components, identifying their responsibilities, and providing a high-level estimate of the work required. During solutioning, special attention is given to non-functional requirements and failover strategies, laying the groundwork for a robust and sustainable technical solution.

- Clearly define the target outcome in measurable terms, allowing for effective comparison and evaluation.
- Articulate specific requirements that must be met by any optimal technical solution.
- Ensure that the solution is sustainable and adaptable to future changes and advancements.

Questions to ask at this stage:

- What is the cost of the solution?
- Are users on Mobile/Desktop/Tablet? 
- Is SEO needed ? 
- Offline support needed?
- Can you deploy each use case independently?
- Do I have clarity on my dependencies? 
- Is it B2B or B2C 
- Is it Consumer Facing or Internal ? 
- Internationalization / Localization support needed ? 

Outcome:
- High-Level solution including system level dependencies and constraints/limitations
- Component Dependencies
- Component Responsibilities
- Rough effort estimates


## Design
The design phase is critical for translating high-level requirements into detailed and actionable plans. This section encompasses both the High-Level Design (HLD) and Low-Level Design (LLD), providing a comprehensive guide for the development team to implement the solution effectively. Additionally, it outlines key design principles and guidelines to ensure consistency and maintainability across the project.

### HLD
The High-Level Design (HLD) phase is a crucial step undertaken by engineering teams to establish a blueprint for component implementation. This process precedes the actual development, ensuring a clear and comprehensive plan before diving into project implementation. 

While the specific considerations may vary based on project nature,The below aspects need to be considered during the HLD phase

- System Architecture & Major Components
- Technology Choice
- Identify Platform - Desktop, Mobile (android, ios), Tablet
- Consumer Facing vs Internal App 
- Performance metrics / Web Vitals / SLA
- Assumptions and Limitations
- Monolithic vs Microfrontend 
- Design Approach: Responsive vs Adaptive Design 
- Mobile first vs Desktop first 
- SSR, CSR, SSG
- SEO Aspects  
- SPA vs MPA
- Security 
- Internationalization (i18n)
- Localization (i10n)
- Accesibility
- State Management
- Qaulity & Test Automation (unit, functional, E2E, Integration etc.)
- A/B Testing 
- Authentication and Authrorization 
- CI/CD, Deployment stretegy
- Logs & Monitoring
- Compliance 
- Analytics & Clickstream 
- Consistency
- Static File Handling & CDN  


Outcome:

**System Architecture**
- Outline the high-level architecture, including major components and their interactions.
- Monolithik, Microfronted Architecture (Iframe, Web Components, Module Federation, Route Based Micro Apps )

**Technology Choice**
- Identify the technology stack, encompassing frameworks, libraries, and development tools.

**Identify User Flow**
- Discuss wireframes and mockups to visualize the layout and structure of the user interface.
- Dicsuss Happy Scenarios, Failing scenarios, Edge Cases 

**Handling API or Communication Protocol**
- Rest APIs, Graph APIs / RPC
- Polling (Short and Long)
- Web Sockets (eg. Chat, Collaborating editors)
- Batching 
- Server Sent Events 
- Caching 

**Credibility & SEO**
- Crawling, Site Ranking, SiteMap
- On Page (Usage of Heading Tags, Semantic Tags, Meta keyword, Title, Performance)
- Off Page (Backlinks, Ads)

**Performance Considerations:**
- Assets Optimisation 
- Delivery Options 
- SLA (Web Vitals, API SLAs)
- Rending Techniques(SSR,SSG,CSR)
- Service workers, Web Workers 

**Security Requirements:**
- CORS, CSP, XSS, CSRF, Clickjacking
- Security Headers 
- HTTPS/SSL
- Authentication & Authorization 
- PII Requirement (Personally identifiable Information)


### LLD

The Low-Level Design (LLD) phase is a detailed exploration of the High-Level Design (HLD), providing in-depth specifications for the component's implementation. This stage involves breaking down the system into smaller, manageable units, ensuring a comprehensive understanding of each module. The LLD addresses specific technical aspects and serves as a guide for developers during the coding phase

While the specific considerations may vary based on project nature,The below are few aspects need to be considered during the LLD phase

- Module Breakdown & Component level use-cases
- Code/Folder Structure 
- UI Component Breakdown 
- State Management 
- API Design & Detailed Interfaces 
- Storage management 
- Routing Management 
- Design System 
- Image Optimisations 
- Assets Optimisations 
- Pagination, Infinite scroll, virtualization
- Deboucing , Throttling 
- Web Vitals: LCP, FCP, TTI, CLS
- Versioning 
- Caching


Outcome:

**Detail Module Specification**
- Comprehensive specifications for each module within the component.

**Elaborate Technology Stack**
- In-depth specifications for the technology stack used.

**UI Component Breakdown**
- Detailed breakdown of UI components, specifying their behavior, interactions, and integration within the overall user interface.

**Design System**
- Implementation of a design system, ensuring consistency in visual elements, typography, and overall user experience.

**Performance Optimizations**
- Buldle size optimisation (Code Splitting, compression etc.)
- Web Vitals (LCP, FCP, TTI, CLS) & Lighthouse Insights
- Caching: Browser caching, API caching, CDN, Disk Cache etc 
- Pagination, Infinite scroll, DOM virtulization 
  
**API Interfaces**
- Well-documented API design with detailed specifications for each interface, facilitating smooth communication between components.


## Technology Choice

The selection of technologies for your frontend system is a critical decision that significantly influences the project's success. It's essential to recognize that each technology comes with its own set of trade-offs, and the suitability of a particular tool or framework depends on the specific context and requirements of your project. 

Here's how to approach the technology choice:

Important points to consider while choosing a Technology or Framework 

**Requirements and Feature**
- Size of project: large / medium / proof of concept 
- Performance Requirements ie Page Load speed etc.
- Look for specific Project requirements such as support for Server side rendering, Mobile support, SPA, User Experience etc

**Coding time and efficiency**
- Speed of development , testing and deployment.
- Ease of use 
- Learning curve 

**Community support and Adoption**
- Strong community support on tools, issues and resolutions
- Battle tested in production (if not a proof of concept)
- Take references of tech usage from big companies to understand if it is being battle-tested. It can be used in production without any worries

**Leverage from what is already available**
- It’s easier to build new applications with the tech we already know so that we do not go through the steep learning curve.

**Flexibility to Scale**
- Assess the level of customization and extensibility provided by the framework. Choose a framework that allows you to tailor the components and styling according to your project's unique requirements.
-  Evaluate how well the framework integrates with other tools, libraries, and development ecosystems, such as build tools, testing frameworks, and state management solutions.

**Documentation and Resources**
- Check the availability of tutorials, guides, and community forums.

**Others**
- Security Considerations: Ensure that the framework or library follows best practices for security.
- License Compatibility: Review the licensing terms of the framework or library to ensure it aligns with your project's licensing requirements and policies.
- Ensure that the framework or library is compatible with the target browsers and devices.

Explore the technology stacks employed by popular companies across various industries on [StackShare](https://stackshare.io/stacks), a platform that provides insights into the tools and technologies utilized to power their applications and services.

## UI Frameworks and Libraries

There are several popular frameworks or Libraries that can be considered/chosen while developing your application. The first step towards making the choice would be to categorize your application based on the requirements first.

| Feature                   | React             | Vue               | Angular           | Svelte            | Web Components    | Next.js           |
|---------------------------|-------------------|-------------------|-------------------|-------------------|-------------------|-------------------|
| **Type**                  | Library           | Framework         | Framework         | Framework         | Technology        | Framework         |
| **Community Support**     | Very High         | High              | Very High         | Growing           | Moderate          | Very High         |
| **Popularity**            | 200,000+ stars    | 180,000+ stars    | 74,000+ stars     | 66,000+ stars     | N/A               | 80,000+ stars     |
| **Scalability**           | Excellent         | Good              | Excellent         | Good              | Good              | Excellent         |
| **Learning Curve**        | Moderate          | Easy              | Steep             | Easy              | Moderate          | Moderate          |
| **Flexibility**           | Highly Customizable | Moderate         | Limited           | Limited           | High              | High              |
| **Performance**           | Good              | Good              | Excellent         | Excellent         | Good              | Good              |
| **Support & Maintenance** | Active            | Active            | Active            | Active            | Varies            | Active            |
| **Compatibility**         | All Browsers      | All Browsers      | All Browsers      | Modern Browsers   | Modern Browsers   | All Browsers      |
| **Integration**           | Excellent         | Good              | Excellent         | Good              | Varies            | Excellent         |
| **Documentation**         | Comprehensive     | Comprehensive     | Comprehensive     | Comprehensive     | Varies            | Comprehensive     |
| **Security**              | Regular Security Audits | Basic Security Measures | Strong Security Practices | Moderate Security Measures | Varies         | Basic Security Measures |
| **License**               | MIT License       | MIT License       | MIT License       | MIT License       | Varies            | MIT License       |
| **Long-Term Viability**   | Active Development | Active Development | Active Development | Active Development | Widespread Adoption | Active Development |
| **User Experience**       | Flexible Components | Reactive Components | Modular Components | Lightweight Components | Depends on Usage   | Depends on Usage   |
| **Feedback & Reviews**    | Positive Reviews  | Positive Reviews  | Mixed Feedback    | Positive Reviews  | Varies            | Positive Reviews  |


### React

#### Pros
- ✅ **Component-Based:** Encourages a modular and reusable component-based architecture.
- ✅ **Virtual DOM:** Optimizes DOM updates for better performance.
- ✅ **Large Community:** Active community and extensive ecosystem of libraries.
- ✅ **React Native:** Allows for mobile app development using React.

## Cons
- ❌ **Learning Curve:** Steeper learning curve, especially for beginners.
- ❌ **Boilerplate Code:** Requires additional setup and boilerplate code.
- ❌ **State Management:** State management can become complex in larger applications.

### Vue

## Pros
- ✅ **Easy to Learn:** Has a gentle learning curve, making it beginner-friendly.
- ✅ **Single-File Components:** Allows encapsulation of components in a single file.
- ✅ **Flexibility:** Can be used for small to large-scale applications.
- ✅ **Vue CLI:** Offers a command-line interface for project scaffolding.

## Cons
- ❌ **Smaller Ecosystem:** Smaller community compared to React and Angular.
- ❌ **Less Mature:** Vue is younger compared to React and Angular.
- ❌ **Corporate Backing:** Less corporate backing compared to React and Angular.


### Angular 
## Pros
- ✅ **Full Framework:** Integrated solution with a comprehensive set of tools.
- ✅ **TypeScript:** Built with TypeScript for static typing and better tooling.
- ✅ **Dependency Injection:** Built-in dependency injection system.
- ✅ **RxJS:** Leveraging reactive programming for managing asynchronous tasks.

## Cons
- ❌ **Steep Learning Curve:** Complex and may take time to learn.
- ❌ **Boilerplate Code:** Requires writing more boilerplate code.
- ❌ **Size of Bundle:** Larger bundle size compared to React and Vue.

### Svelte
## Pros
- ✅ **Compiled Output:** Produces highly optimized and small bundles.
- ✅ **Easy to Learn:** Simple and easy to pick up for developers.
- ✅ **Framework-Integrated:** Minimal boilerplate code and no virtual DOM.
- ✅ **Animation:** Built-in support for smooth animations.

## Cons
- ❌ **Small Ecosystem:** Smaller community compared to React and Vue.
- ❌ **Learning Curve for Web Components:** Specific syntax for building Web Components.
- ❌ **Less Mature:** Svelte is newer compared to React and Vue.

### Next.js

## Pros
- ✅ **React Integration:** Built on top of React, leveraging its benefits.
- ✅ **Server-Side Rendering (SSR):** Provides efficient server-side rendering for improved performance.
- ✅ **Static Site Generation (SSG):** Supports static site generation for fast-loading static pages.
- ✅ **Automatic Code Splitting:** Optimizes and automatically splits code for better performance.
- ✅ **Routing:** Comes with a straightforward and powerful routing system.

## Cons
- ❌ **Learning Curve:** May have a learning curve, especially for beginners.
- ❌ **Opinionated:** More opinionated compared to a vanilla React setup.
- ❌ **Complexity:** For smaller projects, the additional features may introduce unnecessary complexity.
- ❌ **Server Requirements:** SSR may require additional server configurations.

## API Handling and Communication Protocols 

### REST API

#### Pros
- ✅ **Simplicity:** Simple and easy-to-understand design principles.
- ✅ **Stateless:** Stateless interactions, making it scalable and easy to cache.
- ✅ **Uniform Interface:** Consistent conventions for resource manipulation.
- ✅ **Widely Supported:** Supported by a vast array of client libraries and tools.
- ✅ **Caching:** Effective caching mechanisms for improved performance.

#### Cons
- ❌ **Over-fetching or Under-fetching:** Clients might receive more or less data than needed.
- ❌ **Versioning:** Requires careful versioning strategies to avoid breaking changes.
- ❌ **Limited Flexibility:** Can be rigid for certain complex queries or real-time requirements.
- ❌ **Multiple Endpoints:** May require multiple endpoints for various resource manipulations.

### GraphQL

#### Pros
- ✅ **Flexible Query Language:** Clients request only the data they need.
- ✅ **Single Endpoint:** Single endpoint for all operations, reducing network latency.
- ✅ **Real-time Updates:** Supports real-time data with subscriptions.
- ✅ **Strong Typing:** Strongly typed schema for better validation and tooling.
- ✅ **Introspection:** Self-documenting with introspection capabilities.

#### Cons
- ❌ **Learning Curve:** Complex for beginners due to the flexible nature.
- ❌ **Security Concerns:** Potential for malicious queries impacting performance.
- ❌ **Overhead:** Increased payload size due to metadata in responses.
- ❌ **Caching Challenges:** Caching can be more challenging compared to REST.

### WebSockets

#### Pros
- ✅ **Real-time Communication:** Enables bidirectional communication in real-time.
- ✅ **Low Latency:** Reduces latency compared to HTTP-based approaches.
- ✅ **Efficient:** Minimizes overhead and allows for smaller payloads.
- ✅ **Push Notifications:** Supports server-initiated updates to clients.
- ✅ **Full Duplex Communication:** Simultaneous communication in both directions.

#### Cons
- ❌ **Connection Handling:** Requires additional effort to manage and handle connections.
- ❌ **Stateful:** Involves maintaining state on both the client and server.
- ❌ **Firewall Issues:** Can face challenges with firewalls and proxies.
- ❌ **Not Standardized:** No standardized message format or conventions.

### Long Polling

#### Pros
- ✅ **Real-time Updates:** Simulates real-time updates by holding connections open.
- ✅ **Compatibility:** Works well even in environments with limited WebSocket support.
- ✅ **Simple Implementation:** Simpler than WebSocket for basic real-time requirements.
- ✅ **Reduced Server Load:** Reduces the number of open connections compared to WebSockets.

#### Cons
- ❌ **Latency:** Higher latency compared to WebSockets.
- ❌ **Resource Intensive:** Requires maintaining many open connections.
- ❌ **Incomplete Real-time:** Not truly real-time; updates are delayed until the next poll.
- ❌ **Scaling Challenges:** Scaling can become challenging with a large number of clients.

### Server-Sent Events (SSE)

#### Pros
- ✅ **Simplicity:** Simpler than WebSockets for server-to-client communication.
- ✅ **Event Stream:** Supports a unidirectional event stream from server to client.
- ✅ **Browser Compatibility:** Well-supported in modern browsers without additional libraries.
- ✅ **Automatic Reconnection:** Automatic reconnection in case of connection loss.

#### Cons
- ❌ **Unidirectional:** Limited to server-to-client communication.
- ❌ **Limited Browser Support:** Not supported in some older browsers.
- ❌ **No Standardized Error Handling:** Limited error-handling capabilities.
- ❌ **Complex Use Cases:** May not be suitable for more complex real-time requirements.
