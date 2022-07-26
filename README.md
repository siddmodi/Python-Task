First i read the dataframe csv file (Asin,country column) using pandas then create a list named as url_list of all url's by replacing {country} and {asin} in base url of amazon product.
Run a for loop on url_list and using beautifulsoop & requests module we scrap (Product Titile,Product Image URL,Price of the Product,Product Details) for each product url and store values in a dictionary of 4 key-value pairs.
For loop returns a list of dictionaries with 4 key-value pairs.
We append a list with these dictionaries and return URL not available if any url throws Error 404 error.
We also calculated time taken by for loop to end using time module.
At last we jsonify the list by json.dump() method
