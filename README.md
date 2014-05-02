# &lt;current-weather&gt;

> A [Polymer](http://www.polymer-project.org/) element for getting and displaying the current weather at a given location.
> Uses [openweathermap](http://openweathermap.org/API) and [Weather Icons](https://github.com/erikflowers/weather-icons/).

## Demo

[Check it live!](http://dotch.github.io/current-weather)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install current-weather --save
```

Or [download as ZIP](https://github.com/dotch/current-weather/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Custom Element:

    ```html
    <link rel="import" href="bower_components/current-weather/dist/current-weather.html">
    ```

3. Start using it!

    ```html
    <current-weather lat="37.3860500" lon="-122.0838500" units="imperial"></current-weather>
    <current-weather lat="49.27826" lon="11.45929" units="metric"></current-weather>
    ```

## Options

Attribute     | Options     | Default      | Description
---           | ---         | ---          | ---
`lat`         | *double*    | ``           | The latitude of the desired location 
`long`        | *double*    | ``           | The longitude of the desired location 
`units`       | *string*    | `metric'     | 'metric' or 'imperial' units


## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

* To build the distribution files before releasing a new version.

    ```sh
    $ grunt build
    ```

* To provide a live demo, send everything to `gh-pages` branch.

    ```sh
    $ grunt deploy
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

[MIT License](http://opensource.org/licenses/MIT)
