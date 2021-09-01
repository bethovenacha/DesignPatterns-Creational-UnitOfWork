Prerequisite:<br>
Download: Microsoft.EntityFrameworkCore.SqlServer<br>
          Microsoft.EntityFrameworkCore.Design<br>
          Microsoft.EntityFrameworkCore.Tools<br>
          
Unit of work pattern assumes you have a context class that inherits from DbContext class using entity framework core.<br>
You also need to have your domain classes for your project.<br>

1. To use this pattern you need to have the files from this repository included in your project. <br>
2. Instantiate the UnitOfWork class give the domain class as a generic parameter<br>
  e.g. UnitOfWork<YourClass> unit = new UnitOfWork<YourClass>(YourContext);<br>
  
3. Call the method implimented from the repository.
e.g. unit.retrive();<br>
e.g unit.delete(object id);

