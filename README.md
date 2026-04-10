# react-image-gallery

Fork of [xiaolin/react-image-gallery](https://github.com/xiaolin/react-image-gallery). React carousel image gallery component with thumbnail and mobile support.

## Changes from upstream

* Fix crash when gallery is empty
* Add callback on items change
* Add support for not lazy-loading next image
* Improve swipe performance on mobile
* Fix resize handler not updating state with zero value
* Rename `componentWillReceiveProps` to `UNSAFE_componentWillReceiveProps`

## Install

```
npm install @sector-labs/react-image-gallery
```

## Usage

```jsx
import ImageGallery from '@sector-labs/react-image-gallery';

const images = [
  {
    original: 'https://example.com/image1.jpg',
    thumbnail: 'https://example.com/thumb1.jpg',
  },
  {
    original: 'https://example.com/image2.jpg',
    thumbnail: 'https://example.com/thumb2.jpg',
  },
];

<ImageGallery items={images} />
```

### Style import

```scss
@import "~@sector-labs/react-image-gallery/styles/scss/image-gallery.scss";
```

Or without icons:

```scss
@import "~@sector-labs/react-image-gallery/styles/scss/image-gallery-no-icon.scss";
```

## License

MIT
