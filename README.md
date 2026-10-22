# SparkLoop Client API Survey

A static GitHub Pages site that uses the [SparkLoop Client API](https://docs.sparkloop.app/client-api) (`SL.client.surveys`) to fetch a welcome survey with its promotions, render it (including conditional items), and submit the reader's answers and chosen promotions.

## Configuration (URL params)

- `pub` — publication ID (default `pub_6aa6c1374096`)
- `survey` — survey UUID (default `survey_a800a880e760`)
- `test_mode=true` — run in SparkLoop test mode (nothing is recorded). **Without it the page is live** and submissions are real.

The Client API only accepts calls from allowlisted origins, so this site's host (e.g. `<user>.github.io`) must be registered for the publication — otherwise calls fail with `forbidden` (403).
