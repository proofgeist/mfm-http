# mfm-http

A single script that can handle all HTTP requests with Filemaker

Version 2.0.0
Released 3/17/2025

2.0.0 technically has a breaking change but it is highly unlikly to cause problems.
In 1.9.1 we added `response.Ok` property to the response as fast way to check if a response was in the 200 range. Version 2.0.0 changes that to `response.ok`, SO if you never used that feature that is only a couple of months old, you will not be impacted by this change.
