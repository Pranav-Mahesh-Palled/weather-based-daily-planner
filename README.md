# Weather-Based Daily Planner

## Overview

This workflow fetches the current weather for a city, uses Google Gemini to create a personalized daily plan, and sends the result by email.

It suggests outfit ideas, outdoor activities, and weather reminders based on the current conditions.

---

## Problem Statement

People often check the weather and still have to decide:
- what to wear
- whether to go outside
- whether to carry a jacket, umbrella, or sunscreen

This workflow automates that decision-making.

---

## Solution

The workflow:
1. Runs on a daily schedule.
2. Fetches weather data from OpenWeatherMap.
3. Sends temperature, humidity, and description to Gemini.
4. Generates a short daily plan.
5. Emails the plan to the user.

---

## Workflow Architecture

Schedule Trigger  
↓  
OpenWeatherMap API  
↓  
Gemini Daily Planner  
↓  
Gmail Delivery

---

## Technologies Used

- n8n
- OpenWeatherMap API
- Google Gemini
- Gmail
- Schedule Trigger

---

## How It Works

### Step 1: Scheduled Run
The workflow starts automatically every day.

### Step 2: Weather Fetch
It calls the weather API for the selected city.

### Step 3: AI Planning
Gemini uses the weather data to generate:
- outfit suggestion
- outdoor activity suggestion
- weather reminder

### Step 4: Email Send
The plan is sent through Gmail.

---

## Output

A short personalized daily weather plan.

---

## Setup Instructions

1. Import the JSON into n8n.
2. Add your OpenWeatherMap API key.
3. Set your city name.
4. Connect Gmail credentials.
5. Connect Gemini credentials.
6. Activate the workflow.

---

## Future Improvements

- Add more city options
- Add morning and evening versions
- Add calendar integration
- Add Telegram delivery
- Add rain-based alerts

---

## Author

Pranav Mahesh Palled
