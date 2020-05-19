# opt-in-script

Let your website visitors decide whether they want a particular script.

## Usage

```html
<opt-in-script src="analytics.js"
    some-attr="123-456-7">
  <button>Enable analytics!</button>
  Note: this will log foo, bar and baz to my server.
</opt-in-script>
```

The element will be rendered as an unstyled inline element. If the button is clicked, the element is replaced with a corresponding script tag:

```html
<script src="analytics.js" some-attr="123-456-7"></script>
```

This will cause the browser to fetch and run the script.

## Click handler

The click handler will be attached

1. to the first `<button>` inside each `<opt-in-script>`
2. if no button is found, the whole `<opt-in-script>`

## Installation

Recommended:
 1. Review the source code yourself.
 2. Copy `opt-in-script.js` to your site and include it in the end of `<body>`.

Alternatives:
 - `npm install opt-in-script`
 - `<script src="https://cdn.jsdelivr.net/gh/dancek/opt-in-script@0.1.0/opt-in-script.js" integrity="sha384-5EFfPduN0IO9aQmdZGE7hXrteMN54vwjnrln3n12ceFbYRyz4p/vO/UBgaa63tCh" crossorigin="anonymous"></script>`
