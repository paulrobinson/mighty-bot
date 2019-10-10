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

```sh
# Install dependencies
npm install
# Run the bot
npm start
```

## Contributing

If you have suggestions for how mighty-github could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

For more, check out the [Contributing Guide](CONTRIBUTING.md).

## License

[ISC](LICENSE) © 2019 Max Rydahl Andersen <manderse@redhat.com>
