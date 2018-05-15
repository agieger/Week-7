# WEEK 7 - WordPress Pentesting

Time spent: 66 hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Unauthenticated Stored Cross-Site Scripting (XSS)
  - [ ] Summary: you can input an XSS with a comment
    - Vulnerability types:XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
           comment with XSS code on wordpress forum, have the admin approve it, then go to the forum and the XSS will pop up 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
2. Authenticated Cross-Site scripting (XSS)
  - [ ] Summary: there are multiple vulnerabilities in wp-admin/update-core.php You can inject HTML or web script into the names and headers of plugins
    - Vulnerability types: XSS
    - Tested in version:4.2
    - Fixed in version: 4.7.1
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: edit the plugin names with script tags 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
3. Authenticated Stored Cross-Site Scripting (XSS)
  - [ ] Summary:users who are allowed to post on the site can insert HTML with JavaScript on the page by posting. Some configurations would allow unauthenticated users to post or edit content as well.
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: input XSS code into the page or post using HTML editor. The XSS will execute when an admin views the page
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)



## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes


## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
