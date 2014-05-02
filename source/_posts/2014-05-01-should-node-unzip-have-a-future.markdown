---
layout: post
title: "Should Node-Unzip Have a Future?"
date: 2014-05-01 21:18
comments: false
categories: [nodejs, unzip, open source]
---

**_Cross posted from [https://github.com/EvanOxfeld/node-unzip/issues/50](https://github.com/EvanOxfeld/node-unzip/issues/50)_**

I continue to be floored by the response to [node-unzip](https://github.com/EvanOxfeld/node-unzip). While the original implementation was written on a lark, I carried on as a means to better understand streams, arguably the killer feature of NodeJS. Since that time, I've changed companies, ceased personally using this library, and experienced a number of major life events, particularly becoming a father.

I also learned that the zip format is problematic and cannot be perfectly streamed -- see this Apache [doc](http://commons.apache.org/proper/commons-compress/zip.html). That said, if despite the major hangups as well as quality non-streaming NodeJS modules, such as decompress, there's continued interest in this project, I'll work to take the project to a stable 1.0.0, merge outstanding pull requests, and most importantly, seek collaborators who use this library in production.

Thank you and let me know your thoughts on the [project on GitHub](https://github.com/EvanOxfeld/node-unzip/issues/50).
