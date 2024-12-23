# Jelly Backend Tech Test

Welcome! This take-home test is designed to showcase your ability to build a GraphQL API in TypeScript, as well as a
basic React frontend to demonstrate functionality. The aim is to be clear and straightforward. Good luck, and have fun
building!

## Overview

The provided repository is a **React + TypeScript + Vite application** with **Material UI** already configured. It also
contains a `/data` folder with important files you’ll need to complete this test.

### What's in the Repo?

- **React + TypeScript + Vite** project setup
- **Material UI** pre-configured
- `/data` folder containing:
    1. **`ingredients.csv`** – A CSV file with two columns: **ingredient name** and **supplier name**.
    2. **`price_changes.json`** – A JSON file defining **price changes** for each ingredient in the CSV.

## Goal

### 1. Backend (GraphQL + TypeScript)

You’ll build a **GraphQL API** (in TypeScript) that allows you to:

1. **Create and view recipes** through GraphQL queries and mutations.
2. **Recipe structure**:
    - **Name** of the recipe
    - A **collection of ingredients**, each with a specified **quantity (in kg)**
3. **Recipe Cost Calculation**:
    - The API must return the **current cost** of the entire recipe based on the data in `ingredients.csv` and
      `price_changes.json`.

### 2. Frontend (React + Material UI)

You’ll create a basic UI to interact with your GraphQL API. The design does not need to be polished—focus on
functionality. You may use any additional libraries or tools to help you integrate with your API.

Required features:

1. **Create a Recipe**
    - Enter a recipe name
    - Add one or more ingredients (with quantity in kg)
    - Save the recipe through your GraphQL API
2. **View a Recipe**
    - Display the recipe’s name
    - Display a list of ingredients and their quantities
    - Show the **total current cost** of the recipe

## Getting Started

1. **Install Node.js (v20)** – Ensure you have Node 20 on your system.
2. **Install dependencies** – From the project root, run:
   ```bash
   npm install
   ```
3. **Start the application** – Run:
   ```bash
   npm run dev
   ```
   This starts the development server for the frontend.

## Data to Use

- **`ingredients.csv`**  
  Each ingredient has an **ingredient name** and **supplier name**.

- **`price_changes.json`**  
  For each ingredient, there are **price changes** logged with some structure indicating how to calculate or derive the
  current cost.

Your API logic should interpret this data to figure out the **current cost** of each ingredient, which you’ll then use
in calculating the total recipe cost.

## Requirements & Guidelines

1. **GraphQL + TypeScript** – We want to see how you structure a typed GraphQL API.
2. **Recipes** must contain a name and a list of ingredients with quantities (in kg).
3. **Cost Calculation** – The cost must be derived from `ingredients.csv` and `price_changes.json`.
4. **Frontend** – Build any minimal UI you like to:
    - **Add** and **view** recipes
    - **Display** the total cost of each recipe
5. **Feel free to install or use additional packages** to help achieve these goals.
6. **No AI usage** – If at any point you believe AI would help solve a specific problem, please make a note of it and be
   prepared to discuss in your follow-up interview.
7. **Fork or clone** this repo. You can keep the structure or start fresh as long as you **preserve the `/data` folder**.

## Submission

1. **Commit your code** to a **private GitHub repo**.
2. **Add `JackPriceBurns` as a collaborator** so we can access your work.
3. **Send an email** letting us know you’re done and ready for review.

---

**Thank you for taking the time to complete this test. We look forward to seeing what you build!**
