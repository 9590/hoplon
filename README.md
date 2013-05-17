# Hoplon

Hoplon is a set of tools and libraries for making web application front ends.
Hoplon runs entirely on the client and makes no assumptions about the back end
(server side) setup.

### Example

```html
<html>
  <head>
    <title>example page</title>
  </head>
  <body>
    <script type="text/hoplon">
      (ns example.index)
      
      (defn myfn [x y]
        (div {:class "foo"}
          (ul (li x)
              (li y))))
    </script>
    
    <h1>Hello, Hoplon</h1>
    
    <myfn>
      <div>first thing</div>
      <div>second thing</div>
    </myfn>
  </body>
</html>
```

### Dependency

Artifacts are [published on Clojars](https://clojars.org/tailrecursion/hoplon). 
Put this in your _project.clj_:

```clojure
(defproject my-project "0.1.0-SNAPSHOT"
  :plugins      [[thinkminimo/hoplon "0.1.0-SNAPSHOT"]]
  :dependencies [[thinkminimo/hoplon "0.1.0-SNAPSHOT"]])
```

### Demos and Examples

* here
* and here

## License

Copyright © 2012 The Tailrecursion Collective

Distributed under the Eclipse Public License, the same as Clojure.
