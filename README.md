# SSIS


1-Student_Package
----------------
Creating Package that extract data from excel file then apply some transformation like :
1-Character Map : to make the first_name column in upper case.

2-Derived Column : to create new column by concat first_name with last_name to generate full_name column.

3- Copy Column : To copy Dept_id column .

4-Data Conversion : To convert data type of student_id .

5- Sort : To sort students by them ages in desciending order. 

6- Audit : To Genetrate new column with user name of the package . 

After all these transformation , We load the data into Database table .

--------------------------------------------------------------------------------------------------------------------


2-Products_Etl
---------------
Creating Package that extract data from CSV file then apply some transformation like :
1-Data Conversion : To convert data type of Product_id.

2-Lookup : To compare if data in data base or not , the insert un matched data into data base ,
then matched data ,send it into conditional split .

3-Conditional Split : To apply condition (ProductName != Match_ProductName) , If the condition be true then apply
sql command , else apply row sampling . 

4- SQL Command : To apply update statment that get the new product name .

5- Row Sampling : To get random data from data source.
