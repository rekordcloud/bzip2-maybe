# gunzip-maybe

Transform stream that gunzips its input if it is gunzipped and just echoes it if not.

	npm install gunzip-maybe

## Usage

Simply pipe a gzipped (or not gzipped) stream to `gunzip()` and read the unzipped content.

``` js
// this will gunzip gzippedStream
gzippedStream.pipe(gunzip()).pipe(process.stdout);

// this will just echo plainTextStream
plainTextStream.pipe(gunzip()).pipe(process.stdout);
```

## License

MIT