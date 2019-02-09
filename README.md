# ngprobe

Chrome Devetools Elements sidebar to displays Angular Component or AngularJS Scope for selected element i.e. $0.

## How it works

The extension evaluates the following expression in the context of the page and dsiplays the results in ```ngprobe``` sidebar pane :

If Angular is detecetd:

```
    ng.probe($0).componentInstance

    where:

    $0 is the element selected in Elements tab.
```

If AngularJS is detecetd:

```
    angular.element($0).scope()

    where:

    $0 is the element selected in Elements tab.
```

Also shows parent components and scopes as an array.