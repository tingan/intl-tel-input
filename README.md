# International Telephone Input plugin fork with search function[![Build Status](https://travis-ci.org/jackocnr/intl-tel-input.svg)](https://travis-ci.org/jackocnr/intl-tel-input)
A jQuery plugin for entering and validating international telephone numbers with searching phone country code by country name function.

<img src="https://github.com/tingan/intl-tel-input/blob/master/screenshot.png" width="424px" height="246px">
<img src="https://github.com/tingan/intl-tel-input/blob/master/screenshot2.png" width="424px" height="246px">
The work is a by-product from MeetingPackage.com company project [MeetingPackage.com](https://meetingpackage.com).

## Getting Started
1. Download the [latest release](https://github.com/tingan/intl-tel-input/releases/latest), or better yet install it with [npm](https://www.npmjs.com/package/intl-tel-input)

2. Include the stylesheet
  ```html
  <link rel="stylesheet" href="path/to/intlTelInput.css">
  ```

3. Override the path to flags.png in your CSS
  ```css
  .iti-flag {background-image: url("path/to/flags.png");}

  @media only screen and (-webkit-min-device-pixel-ratio: 2), only screen and (min--moz-device-pixel-ratio: 2), only screen and (-o-min-device-pixel-ratio: 2 / 1), only screen and (min-device-pixel-ratio: 2), only screen and (min-resolution: 192dpi), only screen and (min-resolution: 2dppx) {
    .iti-flag {background-image: url("path/to/flags@2x.png");}
  }
  ```

4. Add the plugin script and initialise it on your input element
  ```html
  <input type="tel" id="phone">

  <script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js"></script>
  <script src="path/to/intlTelInput.js"></script>
  <script>
    $("#phone").intlTelInput();
  </script>
  ```

5. **Recommended:** initialise the plugin with the `utilsScript` option to enable formatting/validation, and to allow you to extract full international numbers using `getNumber`.
6. Customization: the search input box style in intlTelInput.scss
```
 #input-search-country {
  width: 400px;
}
```
