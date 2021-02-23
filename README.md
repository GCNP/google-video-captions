# google-video-captions
#### Captions for Videos on Google's YouTube channels

The google-video-captions project has two goals:

* To provide a public corpus of Creative Commons licensed captions that were transcribed from Google videos.
* To enable community-based translation of Creative Commons licensed caption files for these same videos.

The captioned videos are primarily from these Google Developer video channels:

* [GoogleDevelopers](http://www.youtube.com/profile?user=GoogleDevelopers&view=videos)
* [androiddevelopers](http://www.youtube.com/profile?user=androiddevelopers&view=videos)

Not all videos on these channels are captioned. To only see captioned videos, choose the ["Videos with captions"](https://www.youtube.com/playlist?list=PLF8B988C0072C859E) playlist in YouTube.

### Downloading caption files

All captions are stored in the subversion repository for this project. Anyone can view or download these caption files, and reuse is permitted and encouraged under the terms of the [Creative Commons 3.0 BY license](http://creativecommons.org/licenses/by/3.0/). You do not have to be a member of the project to download or view captions.

To view the caption files, choose **Source > Browse**, or [click this link to see the list of English caption files](http://code.google.com/p/google-video-captions/source/browse/trunk/captions/en/).

Alternately, you can check out a copy of all the caption files using a subversion client. See [Checkout](http://code.google.com/p/google-video-captions/source/checkout).

### Finding captioned videos

When you click on a caption file in subversion to see its contents, you will find additional file properties "url" and "title" on the right side of the page. These are the YouTube URL and the video title.

You can get the same information from the subversion command line. For example: 
`svn proplist --verbose google-video-captions/captions/en/*`

### Translating caption files

If you are interested in translating caption files and making them available for others to use, please join this project as a contributor! This will enable you to check files in and out of subversion.

To join the project, send a request to the list http://groups.google.com/group/google-video-captions

To translate and add caption files:

Check out the caption file that you want to translate.
Translate the file.
Save the file under the same name, in a different directory.
Check the translated file in under `google-video-captions/captions/_lang_`, where `_lang_` is the language code. A Spanish translation would be checked in under `google-video-captions/captions/es`.
Set title and url properties to help people find the YouTube video associated with the caption. For example, `svn propset url "http://www.youtube.com/watch?v=HXevnuOOy48" file.srt`

Captions that you upload to this project will be under the same Creative Commons license allowing reuse.

### Uploading caption files to YouTube

Captions can only be added to a video by the channel owner. If you have a translated caption file available for use with a video on the GoogleDevelopers or androiddevelopers channels, please let us know so that we can make it available as a YouTube caption.

1. Send email to google-video-captions@googlegroups.com with a link to the URL of the video in YouTube.
2. We will review the translation for upload to GoogleDevelopers.
3. If we add your translated caption, it will appear when anyone views the video on YouTube with a preference set for that language.

## Wikis
[README](captions/README)

## Original Repo
Migrated from https://code.google.com/archive/p/google-video-captions/

