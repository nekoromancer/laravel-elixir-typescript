elixir-typescript 
========================

**(forked from laravel-elixir-typescript by [MikeyAlder](https://github.com/MikeyAlder/laravel-elixir-typescript))**

## Usage
Check [original version](https://github.com/MikeyAlder/laravel-elixir-typescript)

## Diff
Can use 'sourceMap' option and first argument, outputFileName can be null.

```javascript
  mix.typescript(null, 'public/compiled', '/**/*.ts', {
      target: 'ES5',
      module: 'system',
      moduleResolution: 'node',
      sourceMap: true,
      emitDecoratorMetadata: true,
      experimentalDecorators: true,
      removeComments: false,
      noImplicitAny: false
    });
```

## Parameters

Bellow is the list of the available parameters:

- **outputFileName**: Filename for output
- **outputFolder**(optional): Where to place the output file. Default: `public/js/`
- **search** (optional): filter for input files, can also be a direct path to one file like `app.ts`. Defaults: `/**/*.ts`
- **options** (optional): Options to forward to the `gulp-typescript` used for compiling. All options under https://github.com/ivogabe/gulp-typescript#options
