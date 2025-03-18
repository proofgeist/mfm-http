# mfm-http

A single script that can handle all HTTP requests with Filemaker

## Breaking Change in 2.0.0 - sort of

2.0.0 technically has a breaking change but it is highly unlikly to cause problems.
In 1.9.1 we added `response.Ok` property to the response as fast way to check if a response was in the 200 range. Version 2.0.0 changes that to `response.ok`, SO if you never used that feature that is only a couple of months old, you will not be impacted by this change.

# Version History

## v2.0.1
- **Date:** 3/18/2025
- **Author:** Todd Geist (todd.geist@proofgeist.com)

## v2.0.0
- **Change:** Changed `response.Ok` to `response.ok` to better match standards from other fetch libraries. This is technically a breaking change, which is why the version is updated to 2.0.0. However, it would likely only affect users who started using the `.ok` feature, which probably no one besides the author has.
- **Author:** Todd Geist (todd.geist@proofgeist.com)

## v1.10.1
- **Change:** On FileMaker version 19.5.1 and greater, `content-type=application/json` will be added to the headers if passing JSON data and the header doesn’t already include "application/json".

## v1.9.1
- **Fix:** Resolved an issue with `$error` not being set correctly after the "Insert from URL" step.

## v1.9.0
- **Fix:** Resolved a bug with `application/x-www-form-urlencoded`.
- **Addition:** Added a Boolean "Ok" to the response if the request returns a 200-level response.

## v1.8.0
- **Addition:** Added options for trace and duration.

## v1.7.0
- **Addition:** Added support for nested form fields using `application/x-www-form-urlencoded`.

## v1.6.4
- **Fix:** Resolved an issue with spaces in the username for basic authentication.

## v1.6.2
- **Fix:** Corrected the fix for the empty headers bug.

## v1.6.1
- **Fix:** Fixed an empty headers bug.

## v1.6
- **Enhancement:** Added support for binary and form data.
- **Enhancement:** Added handling for 100 status codes.

## v1.5
- **Date:** 11/12/2018
- **Author:** Todd Geist (todd@geistinteractive.com)
- **Change:** Major refactor based on Generator 1 version.