# Github Action Runner

Basically a word-by-word copy of this great tutorial: https://testdriven.io/blog/github-actions-docker/

## Build

    docker build --tag github_action_runner_image .

    docker run \
      --detach \
      --env ORGANIZATION=<YOUR-GITHUB-ORGANIZATION> \
      --env ACCESS_TOKEN=<YOUR-GITHUB-ACCESS-TOKEN> \
      --name github_action_runner \
      github_action_runner_image
