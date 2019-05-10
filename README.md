
Coming soon..



AWS setup

* Remember to link to the right S3 url and not use the dropdown option in CloudFront
* Gotta invalidate from CloudFront (caches for 24 hours)
  * aws cloudfront create-invalidation --distribution-id $CDN_DISTRIBUTION_ID --paths "/[star]"
  * You could create versioned resources, but you would still have to
    invalidte index.html?
* S3 website has to be public (not writable, of course, but otherwise)


