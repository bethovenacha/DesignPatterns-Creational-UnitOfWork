
Unit of work pattern assumes you have a context class that inherits from DbContext class using entity framework.<br>
You also need to have your domain classes for your project.<br>


0. Include all the files from this pattern.
1. To use this pattern you need to have this classes in your project. <br>
2. Instantiate the UnitOfWork class give the domain class as a generic parameter<br>
  e.g. UnitOfWork<YourClass> unit = new UnitOfWork<YourClass>(YourContext);<br>
  
3. Call the method implimented from the repository.
e.g. unit.retrive();<br>
e.g unit.delete(object id);

