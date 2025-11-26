# @jafps/action-s3

GitHub Action to setup S3.

## Usage

```yaml
name: Pull Request
on:
  push:
    branches: [main]
  pull_request:
    branches: [main]
  workflow_dispatch:

jobs:
  linting:
    runs-on: ubuntu-latest
    steps:
      - name: Setup S3
        uses: jafpsjs/action-s3@v1
        with:
          port: "3900"
          bucket: "bucket"
```
