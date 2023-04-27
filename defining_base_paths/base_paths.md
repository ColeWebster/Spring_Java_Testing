When the @RequestMapping data annotation is used at the class level, the specified path argument will become the base path. 
    - For example, a class with the data annotation @RequestMapping("/books") will map all appropriate requests to this class, and in this case, “/books” becomes the base path. 
    - Methods in this class can be further mapped, as shown in the previous exercise. 
        - In the example shown below, “/books” is now the base path and the getBookThumbnails method is associated with the endpoint “/books/thumbnails”: