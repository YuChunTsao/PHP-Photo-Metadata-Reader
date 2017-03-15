## Synopsis

Photo metadata reader class for PHP that reads the image headers for related metadata.

## Code Example

$meta = new PhotoMetadataReader('/path/to/image/file.jpg');

echo $meta->getTitle(); // title of photo in metadata
echo $meta->getDescription(); // title of photo in metadata

// custom exif array containes the follwing fields: 
// camera_make, camera_model, aperture, exposure, iso, focal_length, flash_fired, flash_value
$custom_exif = $meta->getCustomExif();

## Motivation

This project was created to get a more thurough amount of data from photos than the built in PHP components

## License

MIT