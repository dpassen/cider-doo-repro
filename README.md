# cider-doo-repro

## To exhibit the issue
```sh
lein update-in :dependencies conj \[nrepl/nrepl\ \"0.9.0\"\] -- update-in :dependencies conj \[cider/piggieback\ \"0.5.2\"\] -- update-in :plugins conj \[cider/cider-nrepl\ \"0.27.4\"\] -- update-in :plugins conj \[mx.cider/enrich-classpath\ \"1.5.0\"\] -- update-in :middleware conj cider.enrich-classpath/middleware -- repl :headless :host localhost
```

Then remove the `lein-doo` plugin
