# Web Development

A very small collection of useful web development How-Tos

Index of contents:

1. [Project Checklist](#project-checklist)
* [Security](#security)

## Project Checklist

* Mock-Ups
  Create Mock-Ups for every page in the app and design URLs for each page as well
  Show the design to colleagues and friends for feedback
* Routing
  Setup all routing for app to make sure you can navigate to all URLs you want to create
  Navigate to all URLs you want to create, even if the pages aren't created yet
* Templates & Forms
  Create template & forms
  Make sure they are properly working within the app
* CRUD Functionality
  Add backend functionality and make sure all of the actions on the webpage are
  retrieving data from the database (or any other data source)
  All code operations should work on all pages
* API Endpoints
  Add endpoints that allow the data to be sent if the client requests it in JSON format
  Test API calls within the webbrowser
* Styling & Message Flashing
  Add some CSS, Javascript and images to your application and let it shine

## Security

* Strong Passwords
  Require strong passwords from users to prevent hackers from simply guessing a password 
  and gaining access to private information
* Strong Encryption
  Implement a mathematical algorithm to make information virtually impossible to decrypt
  by someone who doesn't have the right key
* Secure Communication
  Ensure secure communication between client and server to make sure your private information
  doesn't become public at any point along communication
* Password Storage
  Securing password storage in an encrypted database, such that no one can gain access to
  your users password
* Password Recovery
  Implement password recovery, so that if a user forgets their password there's a way to
  create a new one quickly and securely
* Two Factor Authentication
  A highly recommended extra layer of security that requires a password and a special key
  to access private data
* Man-in-the-Middle Attacks
  Protect against the MITM attack to make sure there is no malicious system interfering
  with the data being transmitted or pretending to be a trusted website
