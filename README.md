# Local-business-lead-scraper-n8n
Automated n8n workflow that finds local business leads and writes them to Google Sheets
# Local Business Lead Scraper

An automated workflow that finds local businesses by category and city, cleans the data, and delivers ready-to-use leads directly into a Google Sheet.

## The Problem

Sales teams, marketing agencies, and local businesses often need lists of businesses in a specific category and area — but building that list usually means manually searching Google Maps and copying each entry into a spreadsheet by hand. For a list of 50+ businesses, this can take hours.

## The Solution

This workflow automates the entire process:
1. Searches for businesses by category and location using the Geoapify Places API
2. Cleans the results — removes duplicates and filters out incomplete entries
3. Writes the final list directly into a Google Sheet

Change the category or city, and it runs again for a completely new lead list in under a minute.

## Tech Used

- **n8n** — workflow automation platform
- **Geoapify Places API** — business/location search
- **Google Sheets API** — output destination
- **JavaScript** — data cleaning logic

## How It Works

| Step | Node | What it does |
|------|------|---------------|
| 1 | Trigger | Starts the workflow |
| 2 | HTTP Request | Calls Geoapify Places API with category + location |
| 3 | Code (JavaScript) | Removes duplicates, filters incomplete entries |
| 4 | Clear Sheet | Clears old data before each run |
| 5 | Append Row | Writes clean leads into Google Sheets |

## Example Output

Search: restaurants near Kangra, Himachal Pradesh, India

Returns clean rows with: business name, full address, city, postcode, phone (where available), and coordinates.

## Use Cases

- Sales teams building outreach lists
- Marketing agencies targeting a business category
- Local service providers mapping their delivery area
- Recruiters doing location-based outreach

## Author



https://github.com/user-attachments/assets/4b7f9d0b-32fa-4f03-95d5-59087e8e37bc

Rahul — https://www.linkedin.com/in/rahuljobsdesk/ — automation & data freelancer
