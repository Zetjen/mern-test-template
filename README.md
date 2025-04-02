# Virtual Meeting Slot Reservation System

## Project Description:

The developer should create an application that allows users to reserve one of the available 15-minute meeting slots, with the schedule ranging from 10:00 AM to 3:00 PM. The frontend should allow users to select a time slot and fill out a form with their name and email. This information should then be sent to the backend and stored in MongoDB.

## Task Requirements:

### 1. Frontend:
- Use **Vite** as the bundler for the application.
- Use **MUI (Material UI)** for the user interface, displaying a list of available meeting slots.
- Display the time slots clearly from 10:00 AM to 3:00 PM in 15-minute intervals.
- Each slot should be selectable, opening a form to input the user’s name and email.
- Use **Zod** for form validation on the frontend before sending data to the backend. Required fields include:
  - **Name** (string, required).
  - **Email** (string, required, with valid email format).
- The form should allow multiple reservations for the same slot (non-consumable slots).
- If time permits, implement consumable slots, where each hour can be reserved only once.

### 2. Backend:
- Set up an **Express** server with **MongoDB** to handle reservations.
- Use luxon package to manage time.
- Create a database schema to store reservations.
- For non-consumable slots, allow a time slot to be reserved multiple times.
- If consumable slots are implemented, ensure that each slot can only be reserved once.

### 3. Database:
- Create a **reservations** collection in MongoDB to store the bookings.

## Application Flow:
1. The user will see the available time slots on the frontend (from 10:00 AM to 3:00 PM).
2. After selecting a slot, a form will open to input the user’s name and email.
3. The form data will be validated using **Zod** on the frontend.
4. If the validation is successful, the data will be sent to the backend.
5. The backend will validate the data again and store the reservation in MongoDB.
6. Selected time slots can be reserved multiple times (if non-consumable).
7. If time permits, implement consumable slots where each time slot can only be reserved once.

## Criteria:
- The developer must submit a functional application that allows users to reserve virtual meeting slots.
- The frontend should be clear and easy to use, with proper form validation.
- The backend should correctly handle reservations and store them in MongoDB.
- If consumable slots are implemented, ensure each slot can only be reserved once.
- The developer must follow **Conventional Commits** for commit messages.

## Estimated Time:
Recommended working time is 6 hours, but the developer has the flexibility to take up to 2 working days to deliver the project.
