---
title: Project 1, Iteration 1 wrap-up
date: "2020-01-12"
description: "DNS, SSL, CI/CD; oh man!"
---

Another week down and I couldn't be happier with the progress made. 

When I planned out the project, I created "iterations" with 0 being just creating the app as a single page application and 4 being a finished product with tests, design, and logic. Iteration 0 was simple enough as with the help of hash routers, a single page application with 3 pages was formed. I even found resources explaining how to test routers using Jest and the React Testing Library, so I could complete that iteration. 

Iteration 1 which I am currently on involves adding in the content and logic of the portfolio and hosting the website. The landing page was easy enough as it is just a short welcome with buttons that link to my social media. The project and contact pages have been the hardest part; partly because I tried to over-engineer the solution and partly because I wanted to make something interesting but user friendly.

For the projects page, I grabbed inspiration from dribbble for what would be a neat UX experience for the user. After getting stuck on the implementation for 2 days, I came up with a good middle ground, accordion style blocks. A photo and the title of the project which clicked would reveal below it the description and links to the project. While this was not the exact solution I had envisioned, this kept me sane and for longer description this was a better method then just flipping a card. While this still needs styling, the logic and tests are written which makes me happy.

For the contact page, I looked into creating a form with a react library at first which would send it off to my email address. Researching this way, it seemed to not be that easy or clean so I looked into an almost pure html solution next. I found 2 ways to do it, html on the front end and express.js on the backend or php on the backend. Since I had never used php, I chose the route of express.js and nodemailer. While the theory seems straightforward, I am currently at a roadblock as it was mentioned to POST to a page called send which isn't created (in the walkthrough), I am lost how that is meant to work without a 404. So before I can wrap-up iteration 1, I need to look into more documentation to either solve my errors or to redesign the code in a better way.

Hosting was simple enough. After buying a domain from Google (<a href = "bradleycodes.dev" target="_blank"> bradleycodes.dev </a>), I looked into hosting services with free SSL certification and chose Netlify which is what also hosts this blog. The hardest part has been setting up CI. After looking around and either trying GitHub's workflows, I found the best solution for me would be Travis CI. It offers a completely online experience with a simple script and support for React with a Linux OS. Unfortunately, it isn't as simple as I imagined as tests which pass locally are failing in Travis CI so I might need to optimize the script.

Thank you for taking the time to read this and I will see you on the flip side!