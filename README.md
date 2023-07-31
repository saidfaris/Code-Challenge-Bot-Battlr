# Bot Battlr - React Web App
Welcome to Bot Battlr, the one and only spot in the known universe where you can custom build your own Bot Army! This is an exciting React web application that allows you to browse through a list of robots, view a robot's details, and enlist a bot into your army.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Project Setup](#project-setup)
- [Project Guidelines](#project-guidelines)
- [Core Deliverables](#core-deliverables)
- [Endpoints for Core Deliverables](#endpoints-for-core-deliverables)
- [Advanced Deliverables](#advanced-deliverables)
- [Rubric](#rubric)

## Introduction

This project is a React web application designed to practice various React concepts such as components, props, state, events, and data fetching. The app allows users to view a list of available bots, add individual bots to their army, release bots from their army, and discharge bots permanently.

## Requirements

To successfully run this application, you need to have the following:

- Node.js installed on your machine
- A local server running JSON DB server to fetch data

## Project Setup

Follow these steps to set up the project:

1. Create a new project folder.
2. Create a new GitHub repository and add your Team Manager as a contributor.
3. Regularly commit to the repository to track your progress.
4. In your project directory, create a `db.json` file and use it to set up your local JSON DB server.
5. Run the following command to start the backend server: `json-server --watch db.json`
6. Test your server by visiting this route in the browser: `http://localhost:8001/bots`

## Project Guidelines

Ensure your project adheres to the following guidelines:

- Follow the instructions provided and carefully read the directions for setting up the application.
- Implement all Core Deliverables as outlined below.
- Your app should have a clean and logical code structure.
- Advanced Deliverables are optional, but if attempted, make sure to commit all Core Deliverables first.

## Core Deliverables

As a user, you should be able to:

- See profiles of all bots rendered in the `BotCollection`.
- Add an individual bot to your army by clicking on it. The selected bot should render in the `YourBotArmy` component. The bot can be enlisted only once. It does not disappear from the `BotCollection`.
- Release a bot from your army by clicking on it. The bot disappears from the `YourBotArmy` component.
- Discharge a bot from their service forever, by clicking the red button marked "x", which would delete the bot both from the backend and from the `YourBotArmy` on the frontend.

### DELETE /bots/:id

Example Response:

```json
{}
```

## Advanced Deliverables

These deliverables are optional but are a great way to stretch your skills:

- Choose if you want to enlist a bot into your army or just see their data. Clicking on the card should display a show view (`BotSpecs`) for that bot, which should replace `BotCollection`. BotSpecs should have two buttons: one to go back to the list view and another to enlist that bot.
- Sort bots by their health, damage, or armor using a new component, `SortBar`.
- When you enlist a bot, it should be removed from the `BotCollection` and added to `YourBotArmy`.
- Filter bots by their class, and you can select multiple filters at the same time.
- Sort bots by their health, damage, or armor using