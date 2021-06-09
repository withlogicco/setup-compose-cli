# Set up Docker Compose CLI

GitHub Action making it straightforward to install the desired version of Docker Compsoe CLI.

## Usage

Add the following step in your workflow file

```yml
- uses: parisk/setup-compose-cli@v1
```

### Picking a different version

```yml
- uses: parisk/setup-compose-cli@v1
  with:
    version: 1.0.16
```

---

Built by [Paris Kasidiaris](https://twitter.com/pariskasid) and licensed under the [MIT License](./LICENSE).
