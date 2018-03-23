# Status Report Week 9
## What has been done
Implementation - redone the Dockerfiles to be based on the Rust docker image. Implemented the script semantics in Scala. The cross compiler collects and prints exit code, stdout and stderror to scalas stderr if a external command fails. The idea is to create a cross compiler thread and pipe its stderr to a logfile.

Report - twitched the introduction, make it easier to follow the trail of thought. Written about design and docker.

## Plan for next week
Report - retouch the whole introduction chapter to be almost finished. I also need to reduce the background section about DSLs since it does not seem to relevant for the thesis.

## Not achieved/dropped
Did not implement more docker images.