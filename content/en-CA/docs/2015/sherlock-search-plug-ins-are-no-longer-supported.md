---
title: "Sherlock search plug-ins are no longer supported"
date: "2015-09-23T16:29:00-04:00"
categories: ["misc"]
tags: []
versions: ["44"]
statuses: "affecting"
references:
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=862137"
      title: "Bug 862137 - stop supporting Sherlock search engines"
    - url: "https://bugzilla.mozilla.org/show_bug.cgi?id=862148"
      title: "Bug 862148 - stop supporting installation of Sherlock plugins from the web"
aliases:
    - "/docs/2015/sherlock-search-plugin-is-no-longer-supported/"
---
The support for the legacy Sherlock search plug-in format, [deprecated since Firefox 24](https://www.fxsitecompat.com/en-CA/docs/2013/support-for-sherlock-search-plug-ins-has-been-deprecated/), has been dropped with Firefox 44. The [`window.sidebar.addSearchEngine`](https://developer.mozilla.org/en-US/docs/Adding_search_engines_from_web_pages#Installing_Sherlock_plugins) method now just logs a warning in the Web Console when a Sherlock installation is triggered by Web content.

The `addSearchEngine` method still works for [OpenSearch plug-ins](https://developer.mozilla.org/en-US/Add-ons/Creating_OpenSearch_plugins_for_Firefox), but the [`window.external.AddSearchProvider`](https://developer.mozilla.org/en-US/docs/Adding_search_engines_from_web_pages#Installing_OpenSearch_plugins) method should be used instead as the [`window.sidebar`](https://developer.mozilla.org/en-US/docs/Web/API/Window/sidebar) object will be completely [removed in the future](https://www.fxsitecompat.com/en-CA/docs/2015/window-sidebar-will-be-removed/).
