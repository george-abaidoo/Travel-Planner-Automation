# ✈️ Travel Planner Automation

This project automates **personalized travel planning** by combining weather forecasts, flight data, and reminders using [n8n](https://n8n.io/).  
It’s perfect for frequent travelers who want a smart assistant to simplify trip preparation.

---

## 🚀 Workflow Overview

1. **User Input Form (Webhook)** – User submits travel details (destination, dates, email).  
2. **Flight Info Node (API call)** – Fetches available flights and cheapest options.  
3. **Weather Node** – Pulls weather forecast for the travel dates/destination.  
4. **Google Calendar Node** – Automatically adds trip events (flights, activities).  
5. **Email Summary** – Sends the user a full trip plan with flights + weather.

---

## 📊 Workflow Diagram

    Webhook Form (user submits trip details)
            ↓
        Flight API (fetch flight options)
            ↓
        Weather API (fetch destination forecast)
            ↓
    Google Calendar Node (add trip events)
            ↓
    Email Node (send full trip summary to user)


*Workflow Diagram to be illustrated after full implementation*


---

## 🛠️ Setup Instructions

1. Import the workflow into n8n.  
2. Configure API credentials:
   - Flight data API (e.g., Skyscanner, Amadeus)  
   - OpenWeather API  
   - Google Calendar API  
   - Email account (SMTP)  
3. Submit trip details via the webhook form.  
4. Check your email and Google Calendar for the generated trip plan.

---

## ✅ Example Output

**Email Summary Example:**
>Your Trip to Rome (12–18 March)

>Cheapest Flight: $280 (Delta Airlines)

>Weather Forecast: 18°C average, sunny ☀️

>Events added to your Google Calendar.
