---
title: "`xml:base` attribute has been deprecated"
date: "2017-02-21T20:16:00-05:00"
categories: ["dom"]
tags: []
versions: ["54"]
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=903372"
      title: "Bug 903372 - Remove support for xml:base"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=1340926"
      title: "Bug 1340926 - Add telemetry for xml:base attribute"
    - url: "https://groups.google.com/d/topic/mozilla.dev.platform/1JDnJWefe1E/discussion"
      title: "Intent to unship: xml:base attribute"
---
The [`xml:base`](https://www.w3.org/TR/xmlbase/) attribute in XML documents, that is similar to the [`<base>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/base) element in HTML, is now considered deprecated and will be removed in the near future. It was removed from the spec years ago and no other browsers support it at this time.