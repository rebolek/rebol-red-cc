rebol-red-cc
============

Closed Captioning Files for videos from Rebol and Red Community

There are some crowdsourced websites like [Amara.org]() which are designed to allow people to more organically contribute translations to videos.  So having a GitHub repository may not be the best long-term solution, especially since there will be some redundancy of timing information between the [.SRT](http://en.wikipedia.org/wiki/.srt#SubRip_text_file_format) files.

But this is just a start.  And as a start, the plan is to make a directory for each video project, and then have people put a file in that directory with the language abbreviation and ending in .srt.

Feedback welcome, please feel free to discuss [Rebol and Red chat room](http://rebolsource.net/go/chat-faq)


## Turning Captions on by Default

It can raise the awareness that cpations are available if the captions show up by default, and have to be turned off.  There isn't a checkbox or anything in the YouTube video manager interface to do set this option, the [tricky way of doing it](http://webapps.stackexchange.com/questions/27669/) is to add a tag to your video that says **yt:cc=on**.


## Escaping

If you use Amara to generate closed caption files, it will escape things like quotes as `&quot` or apostrophes as `&#x27;`.  Amara suggests the ability to handle HTML markup, or Markdown, but YouTube will not accept these (at least if you're importing as SRT).  So be sure to fix those up.