# Status Report Week 3
## What has been done
Im still sick but I finished the Rust book. Implemented some trial cases in rust, e.g. dynamically loading libraries which may be used for runtime tools. I have been looking into more DSL background, specially lightweight modular staging (LMS). LMS seems like a good solution, using a staged representation of the task as AST. This work could be split in two, Klas will turn the IR to a staged representation and can possibly add optimizations. I will implement the code generation from staged representation to Rust code. Using generic and traits, the rust compiler will be responsible for generating implementation for actual types in the task.

## Plan for next week
Look into Scala, and further look into background and related work. I would like to extend my writing and understanding of LMS.

## Not achieved/dropped
Nothing