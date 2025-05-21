# java_price_comparator_2025
Spring Boot import from csv price comparator 2025

 To run this application you need to install xampp and create a database named java_price_comparator.
The table products will be created when you first run the java app so you don't need to create it manually
 This app loads data from csv file like the one in the csv folder you can find in this project's root repo directory next to this readme.md file
 The csv data must be separated by coma not semicolon
 In order to test the upload of a new file you need postman and a post call of http://localhost:8085/api/products/upload-csv and in body we select the form-data tab and in file field of File type we get a button to load the .csv file from our computer 

 If the file test_21-05-2025.csv is loaded the store name will be test and loading date will be 21-05-2025. If there where any other data for store test loaded on previous days those will be deleted and the only remaining data 
for store named test will be the data loaded last on 21-05-2025. If on 22-05-2025 we load the latest full data for another store named test2 those will be added to the data loaded on 21-05-2025 for test store. 
