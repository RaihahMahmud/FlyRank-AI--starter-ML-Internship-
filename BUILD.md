# Portfolio Build — Short Build Write-up

## What I Built

I built and deployed a personal portfolio to showcase my software development and machine-learning work, with my FlyRank Machine Learning internship project as the main case study.

The goal was to make it easy for someone unfamiliar with me to understand what I build, see evidence of my work, and access my CV.

## Stack

* React
* Vite
* Tailwind CSS
* Framer Motion
* GitHub
* Vercel

## Why I Chose This Stack

I chose React because I wanted a component-based structure that would be easy to update as I add more projects.

I used Vite for a fast and simple development and production build setup. Tailwind CSS made it easier to control the layout and responsive design without building a large custom stylesheet, while Framer Motion was used for small animations and interactions.

GitHub and Vercel gave me a straightforward workflow from source code to a live deployment.

## The Hardest Thing That Broke

The most difficult issue was getting the production deployment working correctly.

The Vercel build initially failed with a Vite permission error:

`sh: line 1: /vercel/path0/node_modules/.bin/vite: Permission denied`

There was also a separate issue with the CV PDF. The PDF had been corrupted because binary PDF data had been treated as text. The file appeared to exist, but it would not render correctly.

## How I Dealt With It

I first reproduced and checked the build locally instead of assuming the Vercel deployment was the problem.

I cleaned up the project's Git tracking and `.gitignore`, updated the Vite-related dependencies, and verified that the production build completed successfully with `npm run build`.

For the CV, I replaced the corrupted file with the original PDF and verified that the file had a valid PDF header and opened correctly locally. I then committed the corrected file and redeployed it.

The final production build completed successfully, and the deployed CV can now be opened directly from the portfolio.

## What I Would Build Next

My next portfolio case study will be a B2B e-commerce platform.

I want to document it using the same structure:

**Problem → What I did → What came of it**

The project would focus on building a practical business application rather than only demonstrating individual technologies. I also want to explore where machine learning or AI can provide useful functionality within the product.

The goal is to keep building projects that demonstrate both software engineering and practical problem-solving.



# Plan to Keep Building

My next portfolio case study will be a B2B e-commerce platform focused on helping businesses manage products, customers, orders, and other parts of their online sales workflow.

I want to build it as a real software project rather than just a UI demonstration.

## Problem

Small and growing businesses often need a system for managing their products, customers, orders, and sales operations without having to piece together multiple disconnected tools.

The project will explore how a single platform could bring these workflows together in a practical way.

## What I Will Do

I plan to build the platform as a full-stack application, including:

* Product and inventory management
* Business/customer accounts
* Shopping and ordering workflows
* Order management
* Authentication and authorization
* Admin dashboard
* Backend APIs
* Database integration
* Deployment and production infrastructure

I also want to explore where AI or machine learning could provide useful functionality rather than adding AI simply for the sake of using it.

## What I Hope to Get From It

The main outcome will be a deployed, usable application that demonstrates my ability to work across the full software stack.

I will document the project using the same structure as my current case studies:

**Problem → What I did → What came of it**

This will let me show not only the technologies I used, but also the decisions I made, the problems I encountered, and what the finished system actually achieved.

