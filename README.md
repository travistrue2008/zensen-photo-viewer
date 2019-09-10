# zensen-photo-viewer

A photo viewer component for LitElement.

## Features

- Displays image
- Provides multiple content modes
- Provides a way to pan and zoom the photo

## Install

Using `npm`:

```
$ npm install @zensen/photo-viewer
```

Using `yarn`:

```
$ yarn add @zensen/photo-viewer
```

## API

```js
import { IMG_SRC_PORTRAIT } from './_resources'

import { MODE_CONTENT } from '@zensen/photo-viewer'

const ZOOM = 1.5

const PAN_COORDS = {
  x: 16,
  y: 32,
}

const change = src => console.log('viewport src:', src)

... html`
  <zen-photo-viewer
    .mode="${MODE_CONTENT.COVER)}"
    .src="${IMG_SRC_PORTRAIT}"
    .zoom="${ZOOM}"
    .panPos="${PAN_COORDS}"
    .onChange="${change}"
  ></zen-photo-viewer>
`
```
