c64-dragdrop-list
================

See the [component page](http://nzjames.github.io/c64-dragdrop-list) for more information.

## Getting Started

This component is designed to be used with c64-dragdrop.

Standalone example:

```
<c64-dragdrop-list></c64-dragdrop-list>

<script>
    var fileSrc = 'data:image/gif;base64,R0lGODlhAQABAIAAAAUEBAAAACwAAAAAAQABAAACAkQBADs=';

    window.addEventListener('polymer-ready', function(e) {
        document.querySelector('c64-dragdrop-list').fire('file-loaded', {file: null, bin: fileSrc} );
    });
</script>
```

First cut of a drag and drop files target element.

Default behaviour is to listen for `on-file-loaded` event and call the `fileLoaded` handler.
