## Welcome

This is intended to be a simple project to help us get to know your experience with Android development. The goal is to create a simple one screen Android application that can satisfy the following use cases:

1. Display a list of transit stops, sorted by proximity to the user's current location, closest stop first.
2. If the user's current location cannot be obtained, display the stops alphabetized by stop name.
3. For each list item, render what you think is important data from the file. Be prepared to make your case for what should be shown, put yourself in the shoes of a transit user.
4. Ensure that TalkBack announces the stop name using the tts_stop_name column.
5. Support a refresh button. This button should reload the stops and use the user's _latest_ location (if available).
6. Show an error if the stops cannot be loaded.

The transit stops are defined in the included stops.txt file (app/src/main/res/raw/stops.txt). The structure of this file is defined here: https://developers.google.com/transit/gtfs/reference#stopstxt.

The hope is that this takes you a few hours, feel free to take your time and spread the work over a few days.

## Other Requirements

1. Must be written in Kotlin or Java.
2. Must use XML layout.
3. Does not need authentication, localization, unit tests, or UI tests.
4. The stops file must not be loaded on the main UI thread. Be prepared to show or discuss how you would load the same file (or some other representation of the contents of that file) over a network.

## Evaluation

While this is intended to be a relatively simple exercise, carefully consider what libraries, widgets, patterns, and techniques you use. At the same time, avoid over-architecting the application, we consider ourselves pragmatists here at TripShot. Your choices are intended to spark discussion, so if you have ideas for a caching layer, by all means bring it up in a followup discussion, but avoid writing any code for it as part of this exercise.

## Discussion Items

The expectation for the following items is that you search around for some algorithms/approaches. Be prepared to describe an approach you would take, but do not implement them.

1. How could you efficiently find the closest stop given a very large data set?
2. How could you render a large number of stops on a map?
