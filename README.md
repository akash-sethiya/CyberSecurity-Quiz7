# Project 7 - WordPress Pentesting

Time spent: **72** hours spent in total

> Objective: Find, analyze, recreate, and document **three vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) WordPress 3.7-4.4.1 - Open Redirect
  - [X] Summary: 
    - Vulnerability types: Redirect to other target site
    - Tested in version: 3.7
    - Fixed in version: 4.2.7
  - [X] GIF Walkthrough: <img src="https://imgur.com/a/fNaW3" title="Open Redirect Vulnerability Recreate Walkthrough />
  - [X] Steps to recreate: Create a page with title and body and set the onload attribute value to - Some other URL.
  - [X] Affected source code: <body onload="window.location.href = 'www.facebook.com'"></body>
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Unauthenticate Stored Cross Site Scriptiing (XSS)
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: <= 4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: <img src="https://imgur.com/a/EVkjE" title="XSS Walkthrough"></img>
  - [X] Steps to recreate: Create a Page and then added a tag which opens the popup on load of the page, where we can set anything to mess with the user.
  - [ ] Affected source code: The code can be found <a href="">Here</a>
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Required) Unauthenticated Stored Cross Site Scripting (XSS)
  - [X] Summary: 
    - Vulnerability types: XSS
    - Tested in version: <=4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: <img sre="https://imgur.com/a/ol0yB" title="XSS Walkthrough"></img>
  - [X] Steps to recreate: Create a page and then comment on it with unlimited amount of characters which causes the page hand and also write a popup open script on mouse over in the comment and it will keep opening the popup and because of this user would not be able to do anything on the page. Also, any malicious code can be used in the comment in popup code.
  - [X] Affected source code: The code can be found <a href="">Here</a>
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
1. (Optional) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php) 

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2017] [Akash Sethiya]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
