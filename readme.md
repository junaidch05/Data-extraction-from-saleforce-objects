
# ingest_to_db

This script is used to ingest data from Salesforce to a MySQL database. It uses the `simple-salesforce` library to connect to Salesforce and the `mysql-connector-python` library to connect to the MySQL database.

## How to use


1. Update the `SALESFORCE_USERNAME`, `SALESFORCE_PASSWORD`, and `SALESFORCE_SECURITY_TOKEN` environment variables with your Salesforce credentials.
2. Update the `host`, `port`, `user`, `password`, and `database` variables in the `get_database_connection` function with your MySQL database credentials.
3. Run the script by executing `python ingest_to_db.py`
4. The script will connect to Salesforce and retrieve the data from object in dictionary `tables_name`. The script will ingest the data from Salesforce to the MySQL database.

## Note

This script is designed to be run on a daily basis. It will only ingest the data from the previous day. If you want to ingest all the data, you will need to modify the script accordingly.
