## Development

In order to run the website locally, make sure you have Node.js and npm (or a compatible alternative) installed.

### Install dependencies

```shell
npm install
```

### Run locally

```shell
npm run dev
```

### Run locally over local network

Great way to test on a physical mobile device.

```shell
npm run dev -- --host
```

### Build and preview

In order to test a local static build and preview it, you can run the following commands:
```shell
npm run build
npm run preview
```

## Publish

In order to publish, create a PR against the [main](https://github.com/jsafarik/kombuchas/tree/main) branch of this repository. The PR will trigger a [preview](.github/workflows/preview-pr.yml) GitHub workflow, trying to deploy the web to a preview channel.

Once the PR is merged, a [deploy](.github/workflows/deploy.yml) GitHub workflow runs, deploying to a live channel.
