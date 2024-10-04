Employee Dashboard : https://ravitejamoningi.shinyapps.io/EmployeeInfo/  


This app allows users to submit and reset employee details in a simple, centralized form layout.

UI Layout:

The fluidPage() function is used to create a responsive layout.
Custom CSS is added with tags$head() and tags$style() to set a light blue background, ensure full-page height, and center the form in the middle.
The form fields (textInput(), textAreaInput(), selectInput()) are wrapped inside a div container for styling and centered alignment.
The form includes fields for employee information like Name, ID, Contact, Email, Address, Department, Gender, and Message, all styled with black borders and positioned centrally.
Action Buttons:

Two buttons are included: "Submit" and "Clear" using actionButton().
After submitting, the form fields are cleared automatically, and a submission status message is displayed.
Server Logic:

The observeEvent() function listens for the "Submit" button press. It checks for any empty required fields, shows a success message if all fields are filled, and then clears the form.
Another observeEvent() listens for the "Clear" button to reset all fields to their initial empty state.
CSS Styling:

CSS is used to give the form a clean, structured look with black borders, center alignment, and a responsive layout that adjusts to the screen size.   
