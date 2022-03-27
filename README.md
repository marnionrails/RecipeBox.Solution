# Recipe Box

#### By _**Marni Sucher and Brit Wallace**_

#### _An application for users to keep track of recipes._

## Technologies Used

* C#
* .NET 5.0
* dotnet
* MySql/Workbench

## Description

An application for users to keep track of recipes:
Users will be able to:
* add a recipe with ingredients and instructions
* tag recipes with different categories (a recipe can have many tags and a tag can have many recipes)
* update and delete tags to have flexibility with how recipes are categorized
* edit recipes to make improvements or corrections to recipes
* delete recipes and no longer see them as choices
* rate recipes to know which ones are best
* list recipes by highest rated
* see all recipes that use a certain ingredient

## Setup/Installation Requirements

* Make sure you have MySql Workbench installed on your computer.
* Make sure to have dotnet-ef installed too.<br>
<em>This project uses <code>dotnet-ef --version 3.0.0</code> which I have globally installed but you can install it however you want. 
* Download repo: https://github.com/marnionrails/RecipeBox.Solution to your computer using either clone or the download link.
* Open the project in VScode or your terminal/IDE of choice.
* Create a <code>appsettings.json</code> file in the root directory of the project folder. And add the following code replacing anything in square brackets with the information it represents specific to the project database:
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=[DATABASE-NAME-HERE];uid=[USER-ID-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}

```

Example of complete appsettings.json:
```
{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=to_do_list;uid=root;pwd=MySuperStrongPassword;"
  }
}

```
* Make sure to run your mysql server and open MySql workbench.
* Open MySql Workbench and login to your server.
* Click on the Administration tab in the Navigator on the left side of the screen. (this tab will likely be on the bottom of the window)
* In the management section of this administration tab click on the button called <code>Data Import/Export</code>. 
* Once the data import window opens click on <code>Import from Self-Contained file</code> radio button, navigate into the project folder and select <code>recipe_box.sql</code> using the file path next to that radio button.
* Now click on the <code>New...</code> button in the section marked "Default Schema to be Imported To" directly underneath the import options section.
* Click on the "Import Progress" tab at the top of the Data import window.
* At the bottom of this tab click the button that reads <code>Start Import</code>.
* Confirm the database has been imported and you can check it by clicking the "Schemas" tab on the navigator at the left side of the program. Right click in the white space and select "Refresh All"
* Now using your IDE navigate into the RecipeBox.Solution/RecipeBox folder and use the command <code>dotnet run</code> to launch the program. 
* The site should be available at the server address you used in the <code>appsettings.json</code> folder.


## Known Bugs

* _No known bugs_

## Contact Me

Let us know if you run into any issues or have questions, ideas or concerns:  
suchermarni@gmail.com or britwallace888@gmail.com

## License

_MIT_

Copyright (c) _2022_ _Marni Sucher & Brit Wallace_