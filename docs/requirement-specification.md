Temp cue list player - please ignore
====================================

Introduction
------------

Since there are no theatrical cue list players available for Linux, we
decided to write one. This is the product so far.


Definitions
-----------

* Theatrical cue list player - Basically a media player with a
  playlist with some specific requirements. Requirements like
  stability, multiple media clips playing at once, crossfading, clips
  starting at different timings depending on the state of some other
  clip.
* Cue - Something which triggers an event, for example the playback of
  a media clip, or the fade out of such.
* Media clip - Some file which gstreamer is able to playback.
* Cue list - A list of specifications for how media should be played
  back during a show.


System Overview
---------------

The system will consist of a frontend made with QtQuick.

The front end will be controlled by a controller written in Python. This controller has a cue list.

Each cue in the cue list is of a set number of types such as "play a piece of media" or "attenuate the volume".

Music is played.
