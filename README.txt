CS 4241: Webware C25 - Assignment A3 - Aleksandr Samarin - README File

Aleksandr Samarin:

Local Bike Rental Service

For this project I designed a simple website to accept rental bookings for certain types of bicycles.
The idea of the website would be for a user to fill out the form. Then submitting it will display the updated bookings.
Updated from the original design, you now have to sign in through github to be an authenticated user.
User cannot fill out form and see all the bookings unless they are signed in and submit a form.

User can see all rentals and is able to delete the most recent booking until list is empty.
Additionally, the user can modify rental bookings by filling in the form with the same 'Full Name' that they used in the original booking.
This webpage consists of only one .html page but all the technical and design requirements were met.

To run this website, have the project cloned locally on your computer.
Set up a basic npm run configuration selecting 'dev' for the script
Run 'npm run dev'

On preferred browser type URL: 'localhost:3000' OR click link in the server console
This opens up the webpage to use

To actually see what is being added to the database or deleted, you would have to sign in through the sign-in link.

For the secure sign in, I chose the GitHub Passport Strategy so that the user would have to log in through GitHub to access the data.
I chose this method since it was easier to implement and GitHub would handle authenticating users rather than creating new custom user accounts with a seperate login page.

For my CSS. I used Tailwind CSS for the bulk of the styling. I have the tailwind.config.js file as well as the imports in the .html file
I also decided to leave the original styles.css for any original styles for elements on the page.
The positioning technique I used was mostly relative since I used the semantic <header>, <main>, <footer> tags
For the form I also included the flexbox container design to make the layout of the form easier to see on smaller dimensions

The biggest challenges I faced were mainly relating to the secure login strategy through GitHub as well as the Tailwind CSS.
Because I wasn't too familiar with how to use these, configuring them to work in my web application was a bit of trial and error.
Additionally, setting up the server to run on Express gave me some trouble early on, but once I understood what was changing it was not too bad.

Requirements I Met:
    - Server created using Express
    - A results section that will only display the relevant data (excl. pswd) when a user is signed in
    - A form entry that includes the 3 functionalities (ADD, DELETE, MODIFY) associated with the full name provide in the form.

    - Used GitHub Passport Local Strategy to have user sign in, instead of seperate login page.
        - This is more secure as it relies on GitHub to authenticate user and handles any false requests.
    - Used MongoDB as the database to store the app data. Instead of appdata array, all the data goes back and forth from MongoDB Atlas

    - I used Tailwind CSS to style my web application, however I also left my original styles.css to style certain parts of the page.


Technical Achievements
Implement GitHub authentication using either Passport GitHub1 or Passport GitHub2:
    Using the Passport GitHub1 link, I made sure to have the user login via GitHub using the GitHub strategy.

List up to five Express middleware packages you used:
    - mongodb
        -This package is the driver to help connect to the MongoDB Atlas cluster I created.
    - passport
        -This package is used for the secure GitHub login authentication
    - next
        -Using Next.js and tools for full-stack web development and accessing latest React features
    - react
        -This is a necessary package for all React features and elements, used along with web 'react-dom'
    - mime
        -Needed for web applications that serve different types of files.

Design/Evaluation Achievements
No Design Achievements were met for my A3