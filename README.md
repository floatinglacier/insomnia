# Mastercard API Explorer
A customized version of the Insomnia REST Client, which is a cross-platform _REST client_, built on top of [Electron](http://electron.atom.io/). It is customized for {_explorering_|_testing_|_playing with_} Mastercard APIs as a client app without the need to write code for authentication.

## Developing

Development on Insomnia can be done on Mac, Windows, or Linux as long as you have
[NodeJS 8](https://nodejs.org) and [Git](https://git-scm.com/).

<details>
<summary>Initial Dev Setup</summary>

This repository is structured as a monorepo and contains many Node.JS packages. Each package has
it's own set of command, but the most common commands are available from the 
root `[package.json](package.json)` adn can be accessed using the `npm run ...` command. Here
are the only three commands you should need to start developing on the app.

```bash
# Install and Link Dependencies
npm run bootstrap

# Run Tests
npm test

# Start App with Live Reload
npm run app-start
```

</details>

<details>
<summary>Editor Requirements</summary>

You can use any editor you'd like, but make sure to have support/plugins for
the following tools:

- [ESLint](http://eslint.org/) – For catching syntax problems and common errors
- [JSX Syntax](https://facebook.github.io/react/docs/jsx-in-depth.html) – For React components
- [Flow](https://flow.org/) – For type annotations

</details>

## Usage

Add Mastercard API keys by setting a `mastercard` environment variable.

```json
{
	"mastercard": {
		"consumerKey": "[YOUR CONSUMER KEY]",
		"keyAlias": "[YOUR KEY ALIAS]",
		"keystoreP12Path": "[YOUR KEYSTORE .P12 PATH]",
		"keystorePassword": "[YOUR KEYSTORE PASSWORD]"
	}
}
```

## License

[MIT](LICENSE)
