## To Reproduce

2. `yarn install`
3. `docker-compose up`
4. `yarn deploy`
5. `awslocal lambda invoke --function-name=serverless-local-hello /dev/null`
6. `awslocal logs tail "/aws/lambda/serverless-local-hello"`
7. See 'Initialising handler' occur once even if invoked multiple times
8. Add LOCALSTACK_API_KEY to docker-compose.yml environment
9. Repeat steps 3-6
10. See 'Initialising handler occur' for every invocation
