## AWS CLOUDFORMATION COMMANDS
The below commands are use in creating, updating, describing and deleting cloudformation

### Create Stack
```
aws cloudformation create-stack  --stack-name <stack-name> --region us-east-1 --template-body file://<dir-to-ymlfile>
```

### Alternate method to create stack
The below command is also use to create stack with `--parameters file://<dir-to-parammeter>` and `--capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM"`
```
aws cloudformation create-stack --stack-name <stack-name> --template-body file://<dir-to-ymlfile>  --parameters file://<dir-to-parammeter> --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --region=us-east-1
```

### Update stack
```
aws cloudformation update-stack    --stack-name <stack-name> --region us-east-1 --template-body file://<dir-to-ymlfile>
```


###  Describe Stack
```
aws cloudformation describe-stacks --stack-name <satck-name>
```

### Delete Stack 
```
aws cloudformation delete-stack --stack-name <stack-name/>
```
