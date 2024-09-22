# FindComponentsByInterfaces
Utility for Unity that allows you to find components by interfaces.

## Usage
Just write Finder like: ```Finder.FindByInterface<Interface1>().FindByInterface<Interface2>()``` and invoke ```Build()``` method. It will find Components that implement ```Interface1``` and ```Interface2``` interfaces,  and than you can get Components by property or Components as interface by method.

