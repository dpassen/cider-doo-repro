# cider-doo-repro

## To exhibit the issue
```sh
lein update-in :dependencies conj \[nrepl/nrepl\ \"0.9.0\"\] -- update-in :dependencies conj \[cider/piggieback\ \"0.5.2\"\] -- update-in :plugins conj \[cider/cider-nrepl\ \"0.27.4\"\] -- update-in :plugins conj \[mx.cider/enrich-classpath\ \"1.5.0\"\] -- update-in :middleware conj cider.enrich-classpath/middleware -- repl :headless :host localhost
```

Then remove the `lein-doo` plugin

## Additional debug information
```sh
$ lein --version
Leiningen 2.9.8 on Java 11.0.13 OpenJDK 64-Bit Server VM
$ java -version
openjdk version "11.0.13" 2021-10-19
OpenJDK Runtime Environment Temurin-11.0.13+8 (build 11.0.13+8)
OpenJDK 64-Bit Server VM Temurin-11.0.13+8 (build 11.0.13+8, mixed mode)
```
