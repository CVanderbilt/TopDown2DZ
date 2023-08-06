# TopDown2DZ

Below is a mosaic made of GIFs:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Mosaic Made of GIFs</title>
  <style>
    body {
      display: grid;
      grid-template-columns: repeat(2, 1fr) repeat(3, 1fr) repeat(2, 1fr); /* Three columns (2-3-2) with equal width */
      gap: 10px; /* Gap between GIFs */
      justify-items: center; /* Center the GIFs horizontally in each cell */
      margin: 20px;
    }

    img {
      max-width: 100%; /* Ensure the GIFs don't exceed their original size */
    }
  </style>
</head>
<body>
  <!-- First column (2 GIFs) -->
  <img src="https://giphy.com/embed/amTLZka5OMRIYPeMAT" alt="GIF 1">
  <img src="https://giphy.com/embed/h9x0p0B54GG34c2nf5" alt="GIF 2">

  <!-- Second column (3 GIFs) -->
  <img src="https://giphy.com/embed/uIvcg3vg6yoahxDFno" alt="GIF 3">
  <img src="https://giphy.com/embed/FN6Tgb7ZBTGaxvRsZM" alt="GIF 4">
  <img src="https://giphy.com/embed/oFjrnm4FLbhFXuHgzp" alt="GIF 5">

  <!-- Third column (2 GIFs) -->
  <img src="https://giphy.com/embed/PalrIYHVn8Dndaxnuk" alt="GIF 6">
  <img src="https://giphy.com/embed/sXwd0dfFlylEvTSDL4" alt="GIF 7">
</body>
</html>
