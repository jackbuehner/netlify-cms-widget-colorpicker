STILL UNDER CONSTRUCTION
the code is working but the NPM module is not, follow instructions [here](https://github.com/felixboet/netlify-cms-widget-colorpicker/issues/1#issuecomment-695787569) to import the code directly ... and if someone could help to create the NPM module, it would be awesome, I am new to this.

# netlify-cms-widget-colorpicker

A color picker widget for Netlify CMS that supports HEX color codes, alpha channels via RGBA, color names and custom values.

Based on the awesome [react-color](https://casesandberg.github.io/react-color/)

[-> check out the demo here](https://colorpicker-widget.netlify.app/demo)

<img align="center" src="/docs/netlify-cms-widget-colorpicker.gif">

## Install

As an npm package:

```shell
npm install --save netlify-cms-widget-colorpicker
```

```js
import ColorControl from "netlify-cms-widget-colorpicker";

CMS.registerWidget("color", ColorControl);
```

Via `script` tag:

```html
<script src="https://unpkg.com/netlify-cms-widget-color@^0.1.0"></script>

<script>
  CMS.registerWidget("color", ColorControl);
</script>
```

<img src="/docs/netlify-cms-widget-colorpicker-examples.jpg">

## How to use

Add to your Netlify CMS configuration:

```yaml
fields:
  - { name: <fieldname>, label: <fieldlabel>, widget: color }
```

## Configuration

The default color picker is the "chrome picker", you can change it via the options

```yaml
fields:
  - { name: <fieldname>, label: <fieldlabel>, widget: color, picker: github }
```

The following options are available:

```
block
chrome
circle
compact
github
sketch
swatches
twitter
```

##

## Support

For help with this widget, open an [issue](https://github.com/felixboet/netlify-cms-widget-colorpicker)

## Development

Fork the repo, pull the code to your local computer and install dependencies:

```shell
npm install
```

To run a copy of Netlify CMS with the widget loaded for development, use the start script:

```shell
npm start
```

## License

MIT Licensed. Copyright Felix Böttcher

[![Netlify Status](https://api.netlify.com/api/v1/badges/973b0d6d-bb04-412c-b3b1-997fddf42b88/deploy-status)](https://app.netlify.com/sites/colorpicker-widget/deploys)
