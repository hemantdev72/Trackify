Trackify - Amazon Product Price Tracker
Trackify is an Amazon product price tracker that scrapes product prices using Cheerio and monitors price changes. When a product’s price drops below a user-defined threshold, Trackify sends an email notification using Nodemailer. This tool is built with Next.js and runs automated checks with cron jobs.

Features
Amazon Product Scraping: Scrapes product price data from Amazon.
Price Tracking: Monitors the price of selected products.
Email Alerts: Sends email notifications when the price falls below a defined threshold.
Automated Cron Jobs: Periodically checks for price changes.
Tech Stack
Next.js: For server-side rendering and API routes.
Cheerio: For scraping Amazon product data.
Nodemailer: For sending email notifications.
Cron Jobs: For scheduled tasks and periodic price checks.
Installation
Prerequisites
Node.js (v14 or higher)
npm or yarn
Steps
Clone this repository:

bash
Copy
git clone https://github.com/hemantdev72/trackify.git
Navigate to the project directory:

bash
Copy
cd trackify
Install dependencies:

bash
Copy
npm install
Set up your email service with Nodemailer by configuring the .env file:

bash
Copy
SCRAPERAPI_KEY=srcraperapi
MONGODB_URI=mongodburi
EMAIL_PASSWORD=app password of smtp

bash
Copy
npm run dev
Configure your cron job to run the price check periodically (e.g., using node-cron).

Usage
Add products to track by specifying their Amazon URL.
Set the price threshold for receiving email notifications.
The system will automatically check the price and notify you when a price drop occurs.
