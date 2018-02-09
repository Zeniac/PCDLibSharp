# PCDLibSharp
A C# .NET library to read, write and manipulate PCD data files.

This library implements some of the features that are aviliable in the C++ version of the Point Cloud Library https://github.com/PointCloudLibrary

This library is not intended to be a function-by-function C# .NET implementation of the C++ PCD library. While the PCD data format Read and Write functions uses the description given in http://pointclouds.org/documentation/ to be able to load and save PCD files, the code in this library was written from scratch to use the features available in the C# and .Net environments.

The list of features implemented in the lib so far reflects the author's need for them and may never reach the full scope of the C++ PCL library, mostly because the C++ version has several subsystems that are not used by the author, such as the visualization module.

But, if we already have a super complete and well tested PCD library, why create another?

The creator of the lib put it this way: "I've created this library because I needed a way to work with PCD files and data in a .Net application and had no other viable alternative. The original Point Cloud Library doesn't have a .Net version and besides the fact that I wanted/had to work with C# in a .Net application, I didn't want to have to create a wrapper or do other kinds of code juggling to make the C++ version work in my application. Also, as good and useful as they are, the dependencies of the C++ PCD library, like Boost and Eigen, are a nightmare to work with in a managed .Net environment. I wanted all in pure C# managed .Net code."

This codebase follows the old scholl approach of "Do enough design, make it work, then make it fast, then make it beautiful" methodology, also known as circular refinement. If you find that a particular function is not fast or useful enough, it is probably in the 1st or 2nd stages of this coding approach. Justy drop a request and probably there are some places where the code can be improved.
