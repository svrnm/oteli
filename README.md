# ote.li - Short URL Service for the otel & o11y community

[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](http://creativecommons.org/publicdomain/zero/1.0/)
[![Netlify Status](https://api.netlify.com/api/v1/badges/4ce07f1e-b76a-4a74-ac68-82068ef468d3/deploy-status)](https://app.netlify.com/projects/oteli/deploys)

**ote.li** is a short URL service designed for the [OpenTelemetry](https://opentelemetry.io/), observability, and cloud native community. It provides short links for surveys, conference materials, documentation, and other resources. During conferences like Observability Day, KubeCon or OTel Community Day you can replace your generic short URLs with ones that start with `ote.li`!

## Example Redirects

| Short URL | Destination | Purpose |
|-----------|-------------|---------|
| [ote.li/docs](https://ote.li/docs) | OpenTelemetry Documentation | Main docs |
| [ote.li/blog](https://ote.li/blog) | OpenTelemetry Blog | Community blog |
| [ote.li/pr-6820](https://ote.li/pr-6820) | `open-telemetry/opentelemetry.io/pull/6820` | Specific PR reference |

## How to Add Your Own Redirect

Adding a new short URL is driven through Pull Requests:

1. Fork this repository to your GitHub account.
2. Edit the `_redirects` File and add your entry:

    ```text
    /your-path    https://your-destination-url.com    301
    ```

3. Commit your changes & create a new pull request.
4. Review & merge

As an alternative, you can raise an issue to have your link added for you.

## Redirect Guidelines

To maintain quality and consistency, please follow these guidelines:

- Links should be related to OpenTelemetry, observability, or cloud native topics
- Your path should have at least 3 characters.
- Avoid purely commercial content, e.g. a link to your docs _might_ be fine, while to your pricing page will not be accepted.
- Avoid offensive or inappropriate content.

We welcome contributions from:

- Conference speakers sharing talk materials
- Community members conducting surveys
- Project maintainers sharing resources
- Event organizers distributing information

## Technical Details

This service uses Netlify's `_redirects` file format for URL redirection. For advanced
use cases, check [their documentation](https://docs.netlify.com/manage/routing/redirects/overview/).

## License

This project is released under the [CC0 1.0 Universal](LICENSE) license.
