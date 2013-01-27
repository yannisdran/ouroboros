# Ouroboros Sass/CSS Spinner

The Ouroboros is an ancient symbol depicting a serpent or dragon eating its own tail. Inspired by application progress spinners this provides an imageless 'throbber' that eats itself, more or less, for modern browsers.

## Browser Support

Works in Chrome 24+, Firefox 18+, IE 10+, Opera. A standard animated gif is provided as a fall back for older versions of IE.

## Usage

1. For Sass users drop the `_ui-spinner.scss` into your project.
2. Refer to the examples in `example.scss` and use defaults or pass in any arguments.

    @include ui-spinner; // Will use defaults.

    @include ui-spinner(#fff,60px,gray,purple,.7,4s); // Will use these variables.

3. Use with the following HTML:

    <div class="ui-spinner">
        <span class="side side-left">
            <span class="fill"></span>
        </span>
        <span class="side side-right">
            <span class="fill"></span>
        </span>
    </div>

You can also refer to the examples in `index.html`.

The 6 optional parameters:

| Parameter      | Description           | Defaults |
| ------------- |-------------| ----- |
| Hole color*      | Color of the hole to fake a ring | transparent |
| Size      | Size of the spinner      |   46px |
| Background color light | First color, specify a lighter of the two colors      |    #ddd |
| Background color dark | Second color, specify the darker of the two colors      |    #3c76ca |
| Opacity | The opacity of the spinner      |    .8 |
| Duration | Speed of the spinner     |   3s |

The hole color is just to fake a ring spinner. You'd have to match the color you pass here to the background you want to use it against.


## Don't Use Sass?

You can use the CSS that the Sass generates in `stylesheets/main.scss` and make edits to the parameters described above.