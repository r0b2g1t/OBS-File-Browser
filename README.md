OBS-File-Browser
====================

Authors
-------
Francesco Pasqualini  
Nolan Lawson (http://nolanlawson.com)  
Olivier Scherler (http://olivier.ithink.ch/)  

License
-------
GPL v3

Summary
-------

A Bootstrap-y, pretty index.html to be placed at the root of a public Open Telekom Cloud OBS bucket, which
you just want to use for displaying a list of files.

Usage
-----
Edit the bucketUrl variable in the index.html and place the index.html file in the root of your bucket.  It'll look [like this][1].

Setup the following CORS Rule:
 - Allowed Origin: *
 - Allowed Method: GET
 - Allowed Header: *

And allow "Public Read" for your bucket look at [documentation][4].

Changes
-------

### Francesco Pasqualini

[Original version][2].

### Nolan Lawson

- AJAX request and processing using jQuery
- Rendering using Handlebars
- Styling using Bootstrap 2
- User friendly size and date display
- Remove column sorting

### Olivier Scherler

- Support for buckets with more that 1000 (`max-keys`) items
- Bootstrap 3
- Opening and closing folders
- Sort items naturally, ignoring accents
- Item count on folders
- Friendlier date format

### Robert Neumann
- Fixes for use OBS of Open Telekom Cloud
- Parameter integration for filter files
- Add OS reference to title
- Change bucketUrl to Open Telekom Cloud OBS
- Set Telekom template
- Edit README for Open Telekom Cloud


[1]: https://nolanlawson.s3.amazonaws.com/index.html
[2]: https://aws.amazon.com/code/1713
[3]: http://regexp.s3.amazonaws.com/list.html
[4]: https://docs.otc.t-systems.com/en-us/usermanual/obs/en-us_topic_0045853584.html?tag=null
