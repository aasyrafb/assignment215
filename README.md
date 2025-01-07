# assignment215
What is needed to authorize your EC2 to retrieve secrets from the AWS Secret Manager?

1. An IAM role attached to the EC2 instance.
2. The role should have an IAM policy that grants secretsmanager:GetSecretValue permission.
3. Policy should restrict access to the specific secret

Derive the IAM policy (i.e. JSON)?
    -Using the secret name prod/cart-service/credentials, derive a sensible ARN as the specific resource for access

1. arn:aws:secretsmanager:<region>:<account-id>:secret:prod/cart-service/credentials

example
2. arn:aws:secretsmanager:ap-southeast-1:255945442255:secret:prod/cart-service/credentials

