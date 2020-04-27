# create_json_file
imports JSON file from your PhpMyAdmin SQL database (database not included lol)

Okay, what this does is it takes a database table from your phpMyAdmin and dynamically converts that file to JSON.
The JSON file is located within this project.

I needed this to follow my project on pushing data to a JSON file: something that would more easily support an sequential id numbering system for each JSON entry. The ID and the ratings numbers also needed to be 'numbers' (MySQL to JSON makes everything strings, so the variables 'id' and 'ratings' have an (int) prefix (create_json_file.php) so it converts the string to a variable in the final output('ratings.json'). 

![Screen Shot 2020-04-27 at 1 00 42 PM](https://user-images.githubusercontent.com/22375594/80404849-6d10c700-8887-11ea-9a48-7920e0368cde.png)
<img width="666" alt="Screen Shot 2020-04-27 at 1 00 30 PM" src="https://user-images.githubusercontent.com/22375594/80404854-6f732100-8887-11ea-919c-db03c59fe03d.png">


Opening the URL will display the JSON data, and anytime the data is updated on the DB, you can refresh it, 
and it the JSON data will refresh your view and the file data in the .json file (in this case, 'ratings.json')
