# Set up Docker Compose CLI

GitHub Action making it straightforward to install the desired version of Docker Compsoe CLI.

## Usage

Add the following step in your workflow file

```yml
- uses: parisk/setup-compose-cli@v1
```

Now you can use the Docker Compose CLI to deploy your apps to Amazon ECS or Azure Container Instances:

```yml
- uses: parisk/setup-compose-cli@v1
- run: docker context create ecs aws --from-env
- run: docker --context=aws compose up
```
### Picking a different version

```yml
- uses: parisk/setup-compose-cli@v1
  with:
    version: 1.0.16
```

---

Built by [Paris Kasidiaris](https://twitter.com/pariskasid) and licensed under the [MIT License](./LICENSE).
