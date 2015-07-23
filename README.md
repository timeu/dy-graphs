#
# &lt;dy-graphs&gt;

This is a simple Polymer custom element wrapper around [Dygraphs](http://dygraphs.com/)

## Demo
> [Check it live](http://timeu.github.io/dy-graphs/components/dy-graphs/demo/index.html).

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install dy-graphs --save
```

Or [download as ZIP](https://github.com/timeu/dy-graphs/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

  ```html
<script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
  ```

2. Import Custom Element:

  ```html
<link rel="import" href="bower_components/dy-graphs/dy-graphs.html">
  ```

3. Start using it!

  Example with static options:

  ```html
  <template is="dom-bind" id="app">
    <template>
      <dy-graphs data="data.csv" options='{"legend": "always","title": "MyTitle"}'></dy-graphs>
    </template>
  </template>

  ```

  Example with data binding

  ```html
  <dy-graphs data="{{data}}" options="{{options}}"></dy-graphs>
  ```

  Interact with dygraph object directly:

   ```html
    <dygraphs id="graph"></dygraphs>
    <script>
      var g = document.querySelector('#graph');
      g.dygraph.resetZoom();
    </script>
    ```

## Options

See the [component page](http://timeu.github.io/dy-graphs) for more information.


## Browser Support

![IE](https://raw.github.com/paulirish/browser-logos/master/internet-explorer/internet-explorer_48x48.png) | ![Chrome](https://raw.github.com/paulirish/browser-logos/master/chrome/chrome_48x48.png) | ![Firefox](https://raw.github.com/paulirish/browser-logos/master/firefox/firefox_48x48.png) | ![Opera](https://raw.github.com/paulirish/browser-logos/master/opera/opera_48x48.png) | ![Safari](https://raw.github.com/paulirish/browser-logos/master/safari/safari_48x48.png)
--- | --- | --- | --- | --- |
IE 10+ ✔ | Latest ✔ | Latest ✔ | Latest ✔ | Latest ✔ |

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History

Check [Release](https://github.com/timeu/dy-graphs/releases) list.

## License

[MIT License](http://timeu.mit-license.org/) © Ümit Seren