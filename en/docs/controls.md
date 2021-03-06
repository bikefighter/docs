# Tags

Tags (formerly called controls) let you render a view/controller similar to how you would with a template binding.  The main difference is you can pass in attributes as arguments.

Tags start with a ```:``` (colon) to differentiate them from normal html tags.  Like normal html tags, they should be closed.

```html
    <:tag-name />
```

or

```html
    <:tag-name></:tag-name>
```

Refer to the Template Binding section to see how tags lookup their associated view files.  The above has the same lookup as ```{{ template "tag-name" }}```.  Doing ```<:blog:comments />``` is the same as ```{{ template "blog/comments" }}```

A tag loads the same as a template, loading the controller, calling the action method (if one exists), and rendering the view.  You can also pass in attributes to Tags.


