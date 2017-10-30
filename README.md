# fis-parser-dart-sass
A Sass Parser Plugin for FIS, With Dart-Sass

## INSTALL

```bash
npm install -g fis-parser-dart-sass
```

## USE

**fis**

```js
fis.config.set('modules.parser.sass', 'dart-sass');
fis.config.set('roadmap.ext.sass', 'css');
fis.config.set('settings.parser.dart-sass', {
    /* OPTIONS */
});
```

**fis3**

```js
fis.match('*.{sass,scss}', {
    parser: fis.plugin('dart-sass', {
        /* OPTIONS */
    })
});
```

## OPTIONS

- the same API as [node-sass's](https://github.com/sass/node-sass#options)
    - `includePaths`
        - params type is `Array`
        - eg:

            ```js
            /* OPTIONS */
            {
                includePaths: [
                    __dirname + '/xxxx/base'
                ],
            }
            ```
