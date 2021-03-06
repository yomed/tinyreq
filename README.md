
[![tinyreq](http://i.imgur.com/FEAaOq2.png)](#)

# tinyreq

 [![PayPal](https://img.shields.io/badge/%24-paypal-f39c12.svg)][paypal-donations] [![AMA](https://img.shields.io/badge/ask%20me-anything-1abc9c.svg)](https://github.com/IonicaBizau/ama) [![Version](https://img.shields.io/npm/v/tinyreq.svg)](https://www.npmjs.com/package/tinyreq) [![Downloads](https://img.shields.io/npm/dt/tinyreq.svg)](https://www.npmjs.com/package/tinyreq) [![Get help on Codementor](https://cdn.codementor.io/badges/get_help_github.svg)](https://www.codementor.io/johnnyb?utm_source=github&utm_medium=button&utm_term=johnnyb&utm_campaign=github)

> Tiny library for making http(s) requests.

## :cloud: Installation

```sh
$ npm i --save tinyreq
```


:bulb: **ProTip**: You can install the [cli version of this module](http://github.com/IonicaBizau/tinyreq-cli) by running `npm i -g tinyreq-cli`

## :clipboard: Example



```js
const tinyreq = require("tinyreq");

// Make a request to example.com
tinyreq("http://example.com/", (err, body) => {
    console.log(err || body);
});
```

## :memo: Documentation


### `tinyreq(options, callback)`
Creates http(s) requests.

#### Params
- **String|Object** `options`: A string being the request url or an object containing the following fields:
 - `url` (String): The request url.
 - `method` (String): The request method.
 - `data` (Object): The request POST data.
 - `encoding` (String): The encoding type.
- **Function** `callback`: The callback function called (with `error` and `data` parameters).

#### Return
- **EventEmitter** An event emitter you can use for listening for the `data`, `error` and `end` events.



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].

## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:


 - [`cheerio-req`](https://github.com/IonicaBizau/cheerio-req#readme)—An http request module sending back a Cheerio object.
 - [`github-colors`](https://github.com/IonicaBizau/github-colors)—GitHub colors and file extensions mapping
 - [`jsonrequest`](https://github.com/IonicaBizau/jsonrequest)—A tiny library for requesting and getting JSON resources.
 - [`mun`](https://github.com/theuves/mun#readme) (by Matheus Alves)—Obter algumas informações de qualquer município do Brasil.
 - [`tinyreq-cli`](https://github.com/IonicaBizau/tinyreq-cli#readme)—A cli tool for making http(s) requests. CLI for tinyreq.
 - [`wrabbit`](https://github.com/jillix/wrabbit) (by jillix)—Wrap scripts by providing the wrapping function.

## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(http%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: http://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
