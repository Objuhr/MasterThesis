# Status Report Week 9
## What has been done
Implementation - Dockerfile which builds ubuntu image with appropriate linkers and rust/c std library. A script which build the needed images if they don't exist, copies the rust source files to the Docker container, cross compiles to the target platform on the container, and retries the binary executable from the container before shuting it down.

Report - written further about cross compiling and the challanges of cross compiling rust. Written about yarn and containers.

## Plan for next week
Going to have a meeting on monday to show my work.

Implementation - implement docker images for a few more target platforms.

Report - if everythings looks good during the meeting on monday, I will start writing about the design since I now feel like I have comitted to one general design choice.

## Not achieved/dropped
Did not focus on generating code from Klas' tree implementation, this is probably going to be a joint effort.