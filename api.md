# API description

## exact api specification
* Please refer to `http://127.0.0.1:8000/redoc` or the __openapi.json__ file in the directory for the exact specification

## summary
### required
* GET ​/table </br>
Read Table List
* POST ​/table</br>
Create Upload Csvfiles
    * Upload csvfile to sqlite table
        ```
        REQUEST BODY SCHEMA: multipart/form-data
        |- files required
        `--- Array of strings <binary> (Files)
        ```

* GET ​/table​/</br>
Read Table
    * As parameters, table name, filter, column name to be loaded, number of rows to be called, and query result in db
    
        ```
        QUERY PARAMETERS 
        |- table_name required
        |--- string (Table Name)
        |- where	
        |--- string (Where)
        |- select	
        |--- string (Select)
        |- limit	
        `--- integer (Limit)
        ```
    * ex) http://127.0.0.1:8000/table/?table_name=human&where=age%3E30&select=name&limit=1
### appendix
* GET /cache</br>
Read Cache
* GET /cache​/clear</br>
Clear Cache
