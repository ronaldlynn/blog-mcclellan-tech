---
layout: post
title:  "Troubleshooting Firefox MIME Type Errors"
date:   2020-07-04 14:02:18 -0400
categories: firefox
---
* The way Firefox handles 404 errors for CSS and Javascript can be confusing.
* 404s can appear as "The resource from “https://my.url/whatever.css” was blocked due to MIME type (“text/html”) mismatch (X-Content-Type-Options: nosniff).
* This appears to be due to the server returning a 404 page, which is type "text/html".
* Be sure to check the deployment itself, and not just the local resources, to confirm that the file(s) in question were actually deployed.
