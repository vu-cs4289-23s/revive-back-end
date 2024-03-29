# revive-back-end

## File Structure
* `ddb-to-opensearch`: contains the code for the lambda function to stream from database to opensearch.
* `scraper-to-ddb`: contains the code for the lambda function to scrape the web to the database.

## Instructions
### ddb-to-opensearch
To deploy lambda

```
# Install dependencies
pip install --target ./package requests
pip install --target ./package requests_aws4auth

# Zip for deployment
cd package
zip -r ../lambda.zip .
zip -g lambda.zip sample.py
```

### opensearch-api
To deploy lambda

```
# Install dependencies
pip install --target ./package requests
pip install --target ./package requests_aws4auth
pip install --target ./package boto3

# Zip for deployment
cd package
zip -r ../lambda.zip .
zip -g lambda.zip lambda.py
```

### scraper-to-ddb
To deploy lambda

```
# Install dependencies
pip install --target ./package requests
pip install --target ./package bs4

# Zip for deployment
cd package
zip -r ../lambda.zip .
zip -g lambda.zip lambda_function.py
```
