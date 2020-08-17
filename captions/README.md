This folder contains caption files in a variety of different formats.
Some of these formats are not ideal but are included for illustrative
purposes, as YouTube attempts to accept files in whatever formats are
convenient for the users.  However, if you have a choice, we strongly
recommend a format that:

 - Specifies time using fractional seconds, rather than frames.
  SMPTE timecode is problematical because it uses frame counts and
  thus requires knowing the frame rate of the video, which is not
  always possible.
  
   Good:  "00:07:59.16" (0 hours, 7 minutes, 59 seconds, 160 milliseconds)
   
    Bad:  "00:07:59:16" (0 hours, 7 minutes, 59 seconds, 16 "frames")
    
   Ugly:  "00:07:59;16" (drop-frame timecode, implies 29.97HZ)

Also, it is usually best if the format:

- Specifies a duration or stop time, not just a start time.
 If there is only a start time, we have to guess how long to display
 that caption.  You can either rely on our guess, or specify the
 duration explicitly.

For a current description of a simple format that satisfies these
requirements, see this support page:
   http://www.google.com/support/youtube/bin/answer.py?answer=100077
