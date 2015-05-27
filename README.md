Creating a static library for ReactiveCocoa using the Pods repo.

Update the version number in the RACBuilderAggregate build settings to the proper RAC version (Manual for now.)

Build the RACBuilderAggregate for the desired configuration (debug or release).

The output will be in the Derived Data folder. RACBuilder-xxxx->Build->Products->RACBuild

You will see the static library and the Headers folder.

Copy both to your project. 

Link the binary to your target in xcode, and add the path of the "Headers" folder to the headers search path with recursive on (don't add the header files to your project.)


http://www.raywenderlich.com/41377/creating-a-static-library-in-ios-tutorial
http://blog.sigmapoint.pl/automatic-build-of-static-library-for-ios-for-many-architectures/