```
╭───╮╭─╮  
│   ││ │╭─╮╭──┬──┬─╮╭───╮╭───╮   
│   ││ │├─┤│ ╭╮ ╭╮ ││ ─ ││╭╮ │  ╭────────┬─────────────────────╮
╰╮  ╰╯╭╯│ ││ ││ ││ ││  ─┤│╰╯ │  | UPLOAD │ ▒▒▒▒▒▒▒▒▒▒▒░░░░ %75 |                    
 ╰────╯ ╰─╯╰─╯╰─╯╰─╯╰───╯╰───╯  ╰────────┴─────────────────────╯                    
```

[![Build Status](https://travis-ci.org/ecoach-lms/vimeo-upload-js.svg?branch=master)](https://travis-ci.org/ecoach-lms/vimeo-upload)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)
[![GitHub forks](https://img.shields.io/github/forks/ecoach-lms/vimeo-upload-js.svg)](https://github.com/ecoach-lms/vimeo-upload/network)
[![GitHub stars](https://img.shields.io/github/stars/ecoach-lms/vimeo-upload-js.svg)](https://github.com/ecoach-lms/vimeo-upload/stargazers)
[![Percentage of issues still open](http://isitmaintained.com/badge/open/ecoach-lms/vimeo-upload-js.svg)](http://isitmaintained.com/project/ecoach-lms/vimeo-upload "Percentage of issues still open")
> Upload videos to your Vimeo account and update their metadata directly from a browser or a Node.js app.

## Install

Using Bower
```
bower install vimeo-upload
```

Or npm

```
npm install vimeo-upload
```

## Usage

Include `vimeo-upload.js` in your index.html.

```
<script src="bower_components/vimeo-upload/vimeo-upload.js"></script>
```

Create a new `VimeoUpload` initialized with a Blob or File and Vimeo Access Token then call `upload()` to start the upload process.

```javascript
var uploader = new VimeoUpload({
  file: file,
  token: accessToken,
});

uploader.upload();
```

Your access token need to be authorized by Vimeo. Create new Vimeo access token [here](https://developer.vimeo.com/apps).

Check `index.html` for details and additional parameters you can include when initializing `VimeoUpload`.

## Credits

Sample code for uploading files directly with XHR/CORS: [cors-upload-sample](https://github.com/googledrive/cors-upload-sample)
