# DMS db migration to data lake

## Local execution
To testing in the local environment, you need to clone the repository and use the command bellow to deploy the AWS DMS stack. Be sure to set the parameters with staging/development database credentials.

```yaml
sam deploy \
--stack-name test-db-migration \
--template template/dms_migration.yml \
--region us-east-1 \
--capabilities CAPABILITY_IAM \
--parameter-overrides <ALL_PARAMETERS>
```