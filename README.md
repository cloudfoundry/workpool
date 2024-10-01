# Workpool

Use a `WorkPool` to perform units of work concurrently at a maximum
rate. The worker goroutines will increase to the maximum number of
workers as work requires it, and gradually decrease to 0 if unused.

A `Throttler` performs a specified batch of work at a given maximum
rate, internally creating a `WorkPool` and then stopping it when done.

> \[!NOTE\]
>
> This repository should be imported as
> `code.cloudfoundry.org/workpool`.

# Docs

-   [Workpool Example](./docs/010-example.md)

# Contributing

See the [Contributing.md](./.github/CONTRIBUTING.md) for more
information on how to contribute.

# Working Group Charter

This repository is maintained by [App Runtime
Platform](https://github.com/cloudfoundry/community/blob/main/toc/working-groups/app-runtime-platform.md)
under `Diego` area.

> \[!IMPORTANT\]
>
> Content in this file is managed by the [CI task
> `sync-readme`](https://github.com/cloudfoundry/wg-app-platform-runtime-ci/blob/c83c224ad06515ed52f51bdadf6075f56300ec93/shared/tasks/sync-readme/metadata.yml)
> and is generated by CI following a convention.
