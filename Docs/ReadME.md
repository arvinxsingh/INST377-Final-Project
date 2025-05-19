# Developer Manual

This is a developer manual for my  INST377 Final project.  this is a guy that it's intended for future developers who possibly would want to take over the maintenance and development of these pages.  there is a expectation of General understanding of web development Concepts and this documentation will help to walk you through how to install and run this application 
##Overview of project and goals 

The background behind what this project is for is to help people see the current weather within a specific city of their choosing and based upon the current weather be able to tell whether or not they should consider leaving the house earlier or not.  many times within the modern world you're consistently seeing people being laid because of the lack of information that they have.  The idea behind this project is to give people that information in order for them to reach their desired destinations on time.  The project itself allows the users to get real-time weather data  by entering the name of a city and having the temperatures displayed as well as having the specific conditions that are going on within that City. 

The overall goal of the project is create a platform for users to be able to not only get to their desired destination on time but also see the weather conditions that may be affecting their time to their destination.  The hope of this project is to inform users on whether or not they should be leaving early based upon the weather conditions that are currently going on outside. 



## Installation Instructions
When you're first starting off please make sure that you have specific stuff downloaded such as Visual Studio Code, Node.js, Git, Vercel

To get started:
Clone the repository using Git:
    git clone git@github.com:arvinxsingh/INST377-Final-Project.git

Navigate into the project directory
    cd INST377-Final-Project

For this project, most of the app runs using static HTML, CSS, and JavaScript so installation is lightweight

## Running the Application Locally
You have a couple of options to run the project locally:
Using Live Server (recommended for beginners):
    Install the "Live Server" extension in Visual Studio Code

    Opened project in your browser will reflect real-time changes


Using a simple Node server:
    Install the serve package globally by running npm install 

## Supabase API Overview
This application uses Supabase as a to store user data submitted through the form

Setup
The Supabase client is initialized in the Home-page.html file using a public anon key and the Supabase project URL


Database Table Used
Customer_info_project: This table stores customer data submitted via the form, such as first name, last name, and city

The row names are
    customer_first_name
    customer_last_name
    customer_city


Operations being done
    Inserting data: When users submit the form, a POST request is made to insert a new record into the Customer_info_project table.
    Fetching data: A GET request is used to fetch all previous entries, sorted by creation date.



## Known bugs
Supabase Keys are visible on the client side and should be moved to the back side for better security 

There is no user authentication, which means anyone with access to the site can insert data

Weather API keys are exposed and may hit usage limits if too many requests are made

## Future Development Roadmap
For possible future development in order to expand this project, future developers are encouraged to:
    Move all Supabase operations to a secure backend 
    Add robbetter input validation and error handling
    Provide confirmation messages after form submission 
    Add better features such as weather alerts or the ability to search multiple cities



## Folders and what they do
Home-page.html – Homepage is meant to be a landing page in which you are starting up from your application it shows you the 5-day weather forecast for the east coast and it also allows for users to enter their information via a form in order to collect data and send data to the database about who is using the site and where the people are from.

About-page.html – The about page is just a simple page that is meant to describe the purpose of the project and the things that are being used

Project-specific-functionality-page.html – The Project Specific functionality page is a page that is dedicated to showing the main features of the project such as being able to search up the temperature of a specific City and give you a recommendation on whether or not you should leave the house early in order to get to your desired destination on time and efficiently 


Project.css – Cascading style sheets that are used across all the pages

docs/README.md – Documentation file



