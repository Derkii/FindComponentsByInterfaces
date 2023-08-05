# FindComponentsByInterfaces
Utility for Unity that allows you to find components by interfaces.

## Usage
Just write Finder like: ```Finder.FindByInterface<Interface1>().FindByInterface<Interface2>()``` and invoke ```Build()``` method. It will find Components that implement ```Interface1``` and ```Interface2``` interfaces,  and than you can get Components by property or Components as interface by method. Read more in ["Information about under the hood"](https://github.com/Derkii/FindComponentsByInterfaces/edit/main/README.md#information-about-under-the-hood) 

### Information about "under the hood"
```Finder.FindByInterface<TInterface>()``` returns ```FindRequestBuilder``` that also has ```FindByInterface<TInterface>()``` method, so you can use it for write finders.
When you finish to build Finder, use ```Build()``` method that returns FindRequest. 
It gets components in constructor, you shouldn't invoke any methods to do it. Just get components by property, or get components as interfaces by use ```ComponentsByInterface<T>()``` that returns ```IEnumerable<T>```. 

