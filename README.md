# mighty-github

> A GitHub App built with [Probot](https://github.com/probot/probot) that Bot to help maintain your github boards automatically

Initial version based on https://github.com/philschatz/project-bot, with the added benefit it will trigger for updates to issues not just on creation of issues. 

To create an Automation Card, create a Card in a Project like this:

```
###### Automation Rules

<!-- Documentation: https://github.com/maxandersen/mighty-github -->

- `assigned_issue`
- `closed_issue`
- `added_label` **wontfix**
- `new_pullrequest` **repo1** **repo2**
```

## Setup

1. Visit https://smee.io/new and obtian a new Webhook Proxy URL.

2. Edit ``.env`` and set ``WEBHOOK_PROXY_URL=`` the Webhook Proxy URL that you just obtained.

3. Install dependencies:

```sh
npm install
```

4. Now start the application:

```sh
npm start
```

5. Visit  http://localhost:3000/ and click on the "Register GitHub app" button

6. Provide a name for the GitHub app

7. Select where to install the GitHub app

## Contributing

If you have suggestions for how mighty-github could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

For more, check out the [Contributing Guide](CONTRIBUTING.md).

## License

[ISC](LICENSE) © 2019 Max Rydahl Andersen <manderse@redhat.com>
