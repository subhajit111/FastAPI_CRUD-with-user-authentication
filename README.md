execution file:
    - main.py  ------> this contains all the routers of different user url files and database initialization command


database:
    - database.py -----> this file has the database connection commands and function to get database connection


models:
    - models.py -----> this contains the metadata of the tables to be created in the database


userurls and logics:
    - post.py --------> this contains the functions to do crud operation along with urls for the table name Posts
    - users.py -------> this contains the functions to do crud operation along with urls for the table name users


user input and response:
    - schemas.py ------> this contains the schemas of the format of data which has to be followed by the user for input and also response


creating hash(hashing password) and security:
    - util.py -----> this contains the code to secure you password by hashing it and varifying the user by checking the pass they provided


authenticating user login:
    - auth.py ------> this contains the code to authenticate the user by getting his email and password and hashing them
                      aftet it varifies the user then it creates a new token for that user

    - Oauth2.py ----> this contains the code to create the token for the user by encoding the details alsong with secret_key
                      auth.py file calls this file to create the token
                      it also decodes the token given by user and get the data and varifys if that is correct
                      
