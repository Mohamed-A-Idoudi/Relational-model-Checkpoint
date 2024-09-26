# Relational-model-Checkpoint
--Hotel Table:
  -Hotel_Id (Primary Key)
  -Hotel_Name

--Employee Table:
  -Employee_Id (Primary Key)
  -Employee_Name
  -Employee_Speciality
  -Hotel_Id (Foreign Key) – Works for a Hotel

--Type Table:
  -Type_Id (Primary Key)
  -Type_Name
  -Hotel_Id (Foreign Key) – Each room type is associated with a hotel

--Room Table:
  -Room_Id (Primary Key)
  -Floor
  -Type_Id (Foreign Key) – Room type
  -Category_Id (Foreign Key) – Room category

--Category Table:
  -Category_Id (Primary Key)
  -Category_Name
  -Price
  -Beds_Numbers

--Relationships:
  -Hotel–Employee: One hotel has many employees, but an employee works in only one hotel. (Hotel_Id as Foreign Key in the Employee table)
  -Hotel–Type: A hotel has many room types. (Hotel_Id as Foreign Key in the Type table)
  -Room–Type: A room is composed of a specific type. (Type_Id as Foreign Key in the Room table)
  -Room–Category: A room is of a certain category. (Category_Id as Foreign Key in the Room table)
