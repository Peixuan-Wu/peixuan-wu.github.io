## YAML intro

### What is YAML?
YAML (a recursive acronym for “YAML Ain’t Markup Language”) is a data serialization language designed to be human-friendly and work well with modern programming languages for common everyday tasks. This specification is both an introduction to the YAML language and the concepts supporting it. It is also a complete specification of the information needed to develop applications for processing YAML.


### Where is YAML used for?

There are hundreds of different languages for programming, but only a handful of languages for storing and transferring data. Even though its potential is virtually boundless, YAML was specifically created to work well for common use cases such as: configuration files, log files, interprocess messaging, cross-language data sharing, object persistence and debugging of complex data structures. When data is easy to view and understand, programming becomes a simpler task.


## Overview

### Collections
YAML’s block collections use indentation for scope and begin each entry on its own line. Block sequences indicate each entry with a dash and space (“- ”). Mappings use a colon and space (“: ”) to mark each key/value pair. Comments begin with an octothorpe (also called a “hash”, “sharp”, “pound” or “number sign” - “#”).

Example 2.1 Sequence of Scalars (ball players)

- Mark McGwire
- Sammy Sosa
- Ken Griffey



Example 2.2 Mapping Scalars to Scalars (player statistics)

hr:  65    # Home runs
avg: 0.278 # Batting average
rbi: 147   # Runs Batted In


Example 2.3 Mapping Scalars to Sequences (ball clubs in each league)

american:
- Boston Red Sox
- Detroit Tigers
- New York Yankees
national:
- New York Mets
- Chicago Cubs
- Atlanta Braves
  

Example 2.4 Sequence of Mappings (players’ statistics)

-
  name: Mark McGwire
  hr:   65
  avg:  0.278
-
  name: Sammy Sosa
  hr:   63
  avg:  0.288

YAML also has flow styles, using explicit indicators rather than indentation to denote scope. The flow sequence is written as a comma separated list within square brackets. In a similar manner, the flow mapping uses curly braces.


Example 2.5 Sequence of Sequences

- [name        , hr, avg  ]
- [Mark McGwire, 65, 0.278]
- [Sammy Sosa  , 63, 0.288]


Example 2.6 Mapping of Mappings

Mark McGwire: {hr: 65, avg: 0.278}
Sammy Sosa: {
    hr: 63,
    avg: 0.288,
 }