# takecert-dynamodb-tables
The project consists of infrastructure that won't be frequently updated, so it is expected to 
deploy it locally using CLI.

command to deploy dev:
```sh
aws cloudformation deploy --template-file ./template.yaml --stack-name dev-takecert-buckets --parameter-overrides file://dev-parameters.json --capabilities CAPABILITY_NAMED_IAM
```

command to deploy:
```sh
aws cloudformation deploy --template-file ./template.yaml --stack-name takecert-buckets --parameter-overrides file://prod-parameters.json --capabilities CAPABILITY_NAMED_IAM
```