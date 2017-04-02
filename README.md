# Utils.WebAppManager

Import the class and use it like the following:

```cls
// create web app
do ##class(Utils.WebAppManager).Register("/MyWebApp", {
    "Description": ("A sample web application for Cache."),
    "IsNameSpaceDefault": ($$$NO),
    "DispatchClass": (..#DispatchClass)
})

// delete web app
do ##class(Utils.WebAppManager).Delete("/MyWebApp", {
    "DispatchClass": (..#DispatchClass)
})
```

In likely future, this class may appear in Caché package manager.
