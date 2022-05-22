## HairSalon.Solution 

### By Jake Edgar

A web application to keep track of which clients prefer which stylists and vice versa. 

## Tech Used

* C#
* DotNet 
* Razor 
* HTML
* CSS
* Entity Core

## Description 

In this app a user can input a stylist name and specialty and then add clients to their roster. The app is an example of implementing a one to many relationship. 

## Setup/Installation Requirements

* First make sure you have MySql Workbench downloaded and properly installed. You will also need a text editor and a command line that you are comfortable with. 

* In you command line navigate to your desktop directory and clone this project using *Git Clone https://github.com/jakeedgar/HairSalon.Solution.git*

* Open the project in your preferred text editor, I recommend VSCode. 

* To access the database please do as follows:

  * First create a file using the *touch* command in your command line, at the root of the project directory called "appsettings.json" and in that file add the following code, but substituting the text in the brackets for your own information. 

  ```
  { "ConnectionStrings": { "DefaultConnection": "Server=localhost;Port=3306;database=[your_database];uid=[Your ID];pwd=[Your Password];" } }
  ```

* Then open MySQL Workbench and login. 

* Selected the administrator tab and choose "Data Import/ Restore" followed by "Import from self-contained file" Navigate to the directory here, and select "jake_edgar.sql"

* in the tab "Default Schema Imported to" select new, and then name the schema *jake_edgar*.

* The project will not function if the naming convention is not adhered to correctly. 

* Click start to import the file. 

* Refresh the database to make sure synchronization has occurred. 

* In your command line navigate to the directory "HairSalon" and run the following commands in order:
  * *dotnet restore*
  * *dotnet build*
  * *dotnet run*

* Follow the prompt to view the project at *localhost:5000*

## Known Bugs

* There are no known bugs at this time

## License

Licensed under the [MIT License](LICENSE).
Copyright (c) 2022 Jake Edgar