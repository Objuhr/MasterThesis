# Status Report Week 8
## What has been done
Implementation - an inital generator which compiles and macro expands a file generated by the driver then dynamically reflects the resulting class using Scala mirrors and finally emits Cargo.toml, main.rs and lib.rs files. The generator and driver run as seperate threads, it seems a problem to dynamically reload classes using reflection in the jvm. The second time a class is dynamically reflected and loaded to the jvm, the jvm will check if it has loaded it before. And it will find that it has and avoid loading the external definition and supply the already loaded class. Therefore the generator can't reflect the class which is a result of the macro expansion and compilation of the driver generatefd file multiple times. But if the generator runs as a seperate process it gets its own classloader and if it only does one reflection per run the problem is avoided. This means that a new generator process will have to be started for each new ir interpretation. It may be possible to dynamically reload classes using custom classloaders, but it seems low priority and quite complex.

Report - extended the introduction, written about ethics, benefits, and sustainability, and introduction background. The delimitations has been written.
In chapter 2, a part about Meta-Programming and one part about Scala has been started.
Added two figuers, one fore CDA overview and one overview of the code generator.

## Plan for next week
Implementation - start looking how Klas' tree implementation should be merged into the code generator.

Report - look into the "Programming Scala" book, especially the part about reflection, marcos, and string intrepolators. Write part about these capters in the report and explain how they are relevant to the work.

## Not achieved/dropped
None