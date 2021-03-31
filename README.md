<p align="center"><img src="screenshot.svg" alt="Screenshot"></p>
<h3 align="center">Dodgem</h3>
<p align="center">🎪 Rocket League Garage trade bumping automation CLI bot</p>
<p align="center">
	<img src="https://img.shields.io/node/v/dodgem.svg" alt="Minimum Node Version">
    <a href="https://www.npmjs.com/package/dodgem"><img src="https://img.shields.io/npm/dt/dodgem.svg" alt="npm Downloads"></a>
    <a href="https://www.npmjs.com/package/dodgem"><img src="https://img.shields.io/npm/v/dodgem.svg" alt="npm Version"></a>
    <a href="https://github.com/jamieweavis/dodgem/blob/master/LICENSE.md"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
    <a href="https://github.com/airbnb/javascript"><img src="https://img.shields.io/badge/codestyle-airbnb-fd5c63.svg" alt="airbnb Code Style"></a>
</p>

## Installation

**The minimum version of Node.js required to run dodgem is `7.6.0`** - ensure that this version (or higher) is installed before installing dodgem. To check which version of Node.js you have installed you can run: `node -v`.

Dodgem is installed globally via the command line from the npm registry with either [yarn](https://github.com/yarnpkg/yarn) or [npm](https://github.com/npm/npm).

```sh
# Via yarn
$ yarn global add dodgem

# Via npm
$ npm install --global dodgem
```

## Usage

Dodgem is run globally from the command line with the `dodgem` command.

### `dodgem`

Display help and usage information.

### `dodgem login`

Set login credentials for Rocket League Garage.

You will be prompted for your Rocket League Garage email address and password.

### `dodgem start`

Begin the bumping process - you will be prompted for a target and an interval.

Target can be all of your trades _or_ your oldest trade.

All trades is most effective when you have a variety of different active trades - this will bump _all_ of your trades one by one every interval. Oldest trade is most effective when you have lots of duplicate trades and you want to saturate the market - this will bump only your _oldest_ trade every interval.

Interval is the amount of time to wait between bumping. It is recommended to have _atleast_ a 15 minute interval when bumping all trades to prevent bumping too frequently and hitting the 15 minute cooldown timer. When bumping the oldest trade it is recommended to use the following calculation `(15 / amountOfTrades) = interval`.

### `dodgem bump <target> <interval>`

Begin the bumping process but without a prompt for target & interval.

Intended for more advanced users or users who are running multiple instances of Dodgem via `.bat` file for example.

#### `target`

- `all` - For all of your trades
- `oldest` - For only your oldest trade

#### `interval`

Number or decimal of how many minutes to wait between bumps.

## Related

* [Prosper](https://github.com/jamieweavis/prosper) - 💎 Rocket League Garage trade aggregation & reporting CLI tool

## License

This project is licensed under the MIT License - see [LICENSE.md](LICENSE.md) for details.

## Disclaimer

The author and any contributors associated with this project are not resposible for the consequences that may occur from the use of this tool.

Users of this tool do so entirely at their own risk - abusing this tool _could_ get you permanently banned from Rocket League Garage.
