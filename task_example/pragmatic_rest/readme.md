Pragmatic REST Implementation
===
This is an implementation of CRUD pattern for manipulate resources, this is the first step to use the HTTP protocol as an application protocol instead of a transport protocol. 
This protocol follows the level 2 of Richardson Maturity Model.  Basically the API must use a uniform interface, in our case we are using HTTP, so, we need to use the uniform interface provided by HTTP.
This level indicates that your API should use the transport protocol properties in order to deal with scalability and failures. Don't use a single POST method for all, but make use of GET when you are requesting resources, and use the DELETE method when you want to delete a resources. Also, use the response codes of your tunneling protocol. Don't use 200 (OK) code when something went wrong for instance. By doing this for the HTTP transport protocol, or any other transport protocol you like to use, you have reached level 2 - See more at: http://restcookbook.com/Miscellaneous/richardsonmaturitymodel/#sthash.tHyQyI21.dpuf