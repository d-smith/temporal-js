# Temporal JS

A simple temporal project for JavaScript, and by JavaScript I mean TypeScript.

## Misc

Start temporal - temporal server start-dev --db-filename t-dsl.db --ui-port 8080

Temporal can also be run using one of the docker compose versions in the [temporalio/docker-compose](https://github.com/temporalio/docker-compose) repository, for instance:

```bash
docker-compose -f docker-compose-cockroach.yml up
```




Note: first instantiation timeout even after adding a --timeout 20000 flag to the npm test script in package.json

Extending the timeout past 20 seconds yielded:

```
[UnexpectedError: Failed to start ephemeral server: Temp download file at /tmp/temporal-sdk-typescript-1.9.3.downloading not complete after 20 seconds. Make sure another download isn't running for too long and delete the temp file.]
```

Deleting the file and re-running then work, as did subsequent calls.