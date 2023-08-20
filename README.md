# elixir-docker

Automated builder for creating a Docker image eith Erlang and Elixir. This configures Erlang to disable its JIT, a step that is currently necessary when running multiarch Docker builds using Erlang.

Images are built for both amd64 and arm64 and uploaded to the GitHub Container Registry. Currently all images use alpine.

## Docker image

`ghcr.io/extragoodlabs/elixir`

## Tags

The tag format is `{ELIXIR_VERSION}-erlang-{OTP_VERSION}-nojit-{OS}-{OS_VERSION}`.

For example:

- `1.14.5-erlang-25.3.2.3-nojit-alpine-3.18.2`

## License

This repo is licensed under [Apache 2.0](LICENSE).
