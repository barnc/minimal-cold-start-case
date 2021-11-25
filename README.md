## To Reproduce

1. `yarn install`
2. `docker-compose up`
3. `yarn deploy`
4. `awslocal lambda invoke --function-name=serverless-local-hello /dev/null`
5. `awslocal logs tail "/aws/lambda/serverless-local-hello"`
6. `See 'Initialising handler' on every invocation`
