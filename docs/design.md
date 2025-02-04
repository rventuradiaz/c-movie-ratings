# Application Design
## Introduction
### Purpose
To propose a solution design for problem stated in C-movies project 
### Scope
This document will provide a high-level solution, and will not include any code
### Overview
A solution is proposed to read movies data from disparate sources, select the most reliable title, genre, normalise the ratings, calculate the ratings using a proprietary algorithm, and expose the ratings as a web application.
## Requirements
### Functional
FR-01: Source ratings from REST API\
FR-02: Source ratings from CSV via FTP server\
FR-03: Normalise movie ratings\
FR-04: Select the most reliable movie's title\
FR-05: Select the most reliable movie's genre\
FR-06: Calculate C-Rating using total ratings, and ratings by category\
FR-07: Expose C-Movie ratings as a web application accessible through an REST API.\
### Non-functional
NFR-01: Solution shall be DDD compliant.\
NFR-02: Solution design shall follow an agile mindset.\
## Architecture Design
Assumption-01: Entertainment is defined as the Domain (D). Movies is a context (C) withing D. A domain event triggers a request of a movie's info, including a movie's rating.\
Assumption-02: C-Ratings is component of context C, within domain D. C-Ratings is part of movie's root aggregate.\ 
At business level, within domain D, different business users (i.e. a customer, a employee browsing a web page) request information in context C, or a domain event triggered using an agent to refreshing content in context C (see figure 1).\
At application level, different solutions building blocks extract, load, transform, calculate c-rating, and expose the component movies as a REST API (see figure 2).\
### System components and their interactions
### Data flow diagram
### Technology stack
Database server: NoSQL database\
Application server: web application\

## Detailed Design
### Detailed design of each system component
### Class diagrams
### Sequence diagrams
### State diagrams
### Use case diagrams
## Implementation Plan
### Development methodology
### Development environment
### Coding standards
### Testing strategy
### Deployment plan
## Appendix
### Matrices
### Diagrams
#### Figure 1. Bizz architecture diagram
[<img src = "Bizz architecture.bmp">]
#### Figure 2. App architecture diagram
[<img src = "App architecture.bmp">]
