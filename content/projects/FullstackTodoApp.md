---
title: "Fullstack Todo List App"
featured: true
summary: "Built with Next.js (frontend) and Express.js + PostgreSQL (backend), this app lets users create, organize, and manage tasks in real-time. Features include task grouping, due dates, and user authentication with sessions. Styled using Tailwind CSS and component libraries for a clean, responsive UI."
imagePath: "/images/fullstacktodo.png"
videoPath: "https://www.youtube.com/embed/88C6PFBwNkY?si=GVrwNYmpkqcNOG_u"
weight: 1000
categories:
- Web Dev
tags:
- Full-Stack
- React
- Express.js
- PostgreSQL
- Node
- Next.js
- JavaScript
- TypeScript
- Relational Database
draft: false
---

### Links
- [Front-end Source](https://github.com/erikbolumburu11/todolist-client)
- [Back-end Source](https://github.com/erikbolumburu11/todolist-server)
- [Demo Link](https://bolumburutodolist.netlify.app/)

### Features
- Task Management
- JWT Authentication System
- Responsive Design
- Due Dates
- Task Sorting
- Task Grouping

### Front-end
The front-end is built using Next.js (TypeScript) and styled using Tailwind CSS. I used many components from [shadcn/ui](https://ui.shadcn.com/) and used [TanStack Table](https://tanstack.com/table/latest) for the todo list. [React Hook Form](https://www.react-hook-form.com/) along with [Zod](https://zod.dev/) for schema validation was also used.

### Back-end
The Back-end is built using Express.js (JavaScript) and connects to a PostgreSQL relational database. Authentication was previously implemented using Passport.js (with hashed passwords) and Express Session, however was overkill for the use case and wouldn't allow mobile users to authenticate easily, so the authentication system was refactored to use JWT (JSON Web Tokens) authentication instead.

### Deploying
To deploy my front-end, I used [Netlify](https://www.netlify.com/) and to deploy my back-end I used [Render](https://render.com/). The Postgresql database is hosted on [Neon](https://neon.com/). Fortunately all of these services are free!

### CI/CD
Whenever changes are pushed to the master branch of either the client or server repositories, Netlify or Render will build and redeploy the projects automatically.