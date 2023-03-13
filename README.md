### Launch EC2 instance
- Image AMI: `ami-0cdf84c392db3c246` (RHEL 9)
- Also create inbound ssh rule to allow ssh in
- Requires to have created a keypair named `Ec2Master`

### Run
```
aws cloudformation deploy --template-file template.yaml --stack-name Ec2Rhel --output json
```

### Destroy
```
aws cloudformation delete-stack --stack-name Ec2Rhel
```

