# Git flags Buildkite Plugin

Sets the Buildkite git flags for the current build.

## Example

Add the following to your `pipeline.yml`:

```yml
steps:
  - command: ls
    plugins:
      - Hivebrite/git-flags#v0.0.1:
          clone: "--all"
          fetch: "--all"
```

## Configuration

### `clone` (Optional, string)

Git clone flags, for example `--all`. Supports any pattern supported by [git clone](http://man7.org/linux/man-pages/man1/git-clone.1.html).

### `fetch` (Optional, string)

Git fetch flags, for example `--all`. Supports any pattern supported by [git fetch](http://man7.org/linux/man-pages/man1/git-fetch.1.html).

## Developing

To run the tests:

```shell
docker-compose run --rm tests
```

## Contributing

1. Fork the repo
2. Make the changes
3. Run the tests
4. Commit and push your changes
5. Send a pull request
