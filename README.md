# Geolocation Validator

The Geolocation Validator package provides a set of methods to validate
the location of a device based on its geographical coordinates, allowing
you to implement location-based access control in your applications.
Whether you want to ensure that users are within a specific area before
granting access or validate device locations, this package simplifies
the process.

## Installation

You can install the Geolocation Validator package using npm, yarn, or
bower.

Using npm:

`npm install geolocation-validator --save`

Using yarn:

`yarn add geolocation-validator`

Using bower:

`bower install geolocation-validator --save`

## Usage

Here's how you can use the Geolocation Validator package in your
JavaScript or TypeScript code:

```javascript
import { GeoLocationValidator } from "geolocation-validator";

// Create an instance of the GeoLocationValidator
const geoLocator = new GeoLocationValidator();

// Define the coordinates of the device you want to validate
const myCoordinates = {
  latitude: 4.825979675576107,
  longitude: 7.05675985088703,
};

// Define the coordinates of the point of validation
const pointOfValidation = {
  latitude: 7.05675985088703,
  longitude: 4.825979675576107,
};

// Validate the device's location
const validated = await geoLocator.validateLocation(
  myCoordinates,
  pointOfValidation,
  0
);
```

**Output:**

```javascript
{
   result: false,
   message: 'Device is not presently within the range of validation'
}
```

## Documentation

For comprehensive documentation, including detailed API reference and
usage examples, visit the
[official documentation](https://michael2004-ukpeh.github.io/geolocation-validator/).

## Contribution

We welcome contributions from the open-source community. If you'd like
to contribute to the Geolocation Validator package, please check out the
[GitHub repository](https://github.com/Renaissance-Innovation-Labs/Location-Checker.git)
and follow our [contribution guidelines](CONTRIBUTING.md).

Feel free to modify and expand this README file to provide more
information about your package, its features, and how to use it
effectively. Additionally, make sure to update the links and
placeholders with the actual links and content from your project.
