Clojure landscape from Java perspective
=======================================

This list shows Clojure equivalents to popular Java/JavaScript libraries and frameworks. It should be helpful for people transitioning from Java to Clojure (I'm one of those).

In concept it is similar to
[mongo to sql comparision](http://docs.mongodb.org/manual/reference/sql-comparison/) and [intellij for eclipse users](https://www.jetbrains.com/idea/help/eclipse.html) guides. So it tells you what are to new ways of doing what you already know.

Most technologies/concepts has been taken from [JHipster technology stack](https://jhipster.github.io/tech_stack.html).

**Pull requests welcome!**

Backend
-------

| Java | Clojure |
|------|---------|
|[JHipster](https://jhipster.github.io/)|[luminus](http://www.luminusweb.net/)|
|[Maven](https://maven.apache.org/), [Gradle](https://gradle.org/) | [leiningen](http://leiningen.org/) |
|[Spring](http://projects.spring.io/spring-framework/) | [component](https://github.com/stuartsierra/component), [system](https://github.com/danielsz/system) |
|[Spring Boot](http://projects.spring.io/spring-boot/) | [duct](https://github.com/weavejester/duct), [modularity](https://modularity.org/templates/hello-world-web.html), [mr-clojure](https://github.com/mixradio/mr-clojure), [compojure-api](https://github.com/metosin/compojure-api), [tesla-microservice](https://github.com/otto-de/tesla-microservice)|
|[Spring MVC](http://docs.spring.io/spring-framework/docs/current/spring-framework-reference/html/mvc.html)|[compojure](https://github.com/weavejester/compojure), [compojure-api](https://github.com/metosin/compojure-api)|
|WebSockets|[sente](https://github.com/ptaoussanis/sente), [chord](https://github.com/jarohen/chord), [gniazdo](https://github.com/stylefruits/gniazdo)|
|[Jackson](http://wiki.fasterxml.com/JacksonHome)|[cheshire](https://github.com/dakrone/cheshire)|
|[Thymeleaf](http://www.thymeleaf.org/)|[enlive](https://github.com/cgrand/enlive), [hiccup](https://github.com/weavejester/hiccup), [selmer](https://github.com/yogthos/Selmer)|
|[JAWR](https://jawr.java.net/)|[optimus](https://github.com/magnars/optimus)|
|Bean Validation|[schema](https://github.com/Prismatic/schema), [validateur](https://github.com/michaelklishin/validateur), [bouncer](https://github.com/leonardoborges/bouncer), [verily](https://github.com/jkk/verily)|
|[Logback](http://logback.qos.ch/)|[timbre](https://github.com/ptaoussanis/timbre)|
|[OkHttp](http://square.github.io/okhttp/), [Apache Http Client](https://hc.apache.org/httpcomponents-client-ga/)|[clj-http](https://github.com/dakrone/clj-http), [http-kit client](http://www.http-kit.org/client.html)|
|[JUnit](http://junit.org/)/[AssertJ](http://joel-costigliola.github.io/assertj/)|[clojure.test](http://blog.jayfields.com/2010/08/clojuretest-introduction.html), [humane-test-output](https://github.com/pjstadig/humane-test-output), [midje](https://github.com/marick/Midje), [expectations](http://jayfields.com/expectations/)|
|[Wiremock](http://wiremock.org/)|[clj-http-fake](https://github.com/myfreeweb/clj-http-fake)|
|[Spring Security](http://projects.spring.io/spring-security/)|[friend](https://github.com/cemerick/friend), [buddy](https://github.com/funcool/buddy/)|
|[Spring Data](http://projects.spring.io/spring-data/)|[system](https://github.com/danielsz/system)|
|JPA|[korma](http://sqlkorma.com/)|
|[JDBI](http://jdbi.org), [JOOQ](http://www.jooq.org/)|[honeysql](https://github.com/jkk/honeysql), [yesql](https://github.com/krisajenkins/yesql)|
|[Liquibase](http://www.liquibase.org)|[ragtime](https://github.com/weavejester/ragtime), [migratus](https://github.com/yogthos/migratus)|
|[Quartz](http://quartz-scheduler.org/)|[quartzite](https://github.com/michaelklishin/quartzite), [chime](https://github.com/jarohen/chime)|
|[JRebel](http://zeroturnaround.com/software/jrebel/), [Spring loaded](https://github.com/spring-projects/spring-loaded)|[reloaded.repl](https://github.com/weavejester/reloaded.repl)|

Frontend
--------

|Javascript|ClojureScript|
|----------|-------------|
|[Grunt](http://gruntjs.com/)|[leiningen](http://leiningen.org/), [boot](http://boot-clj.com/)|
|[Yeoman](http://yeoman.io/)|[chestnut](https://github.com/plexus/chestnut), [tenzing](https://github.com/martinklepsch/tenzing)|
|[grunt live reload](https://github.com/gruntjs/grunt-contrib-watch#optionslivereload)|[figwheel](https://github.com/bhauman/lein-figwheel)|
|[Angular](https://angularjs.org/)| [om](https://github.com/omcljs/om)/[reagent](https://github.com/reagent-project/reagent)/[quiescent](https://github.com/levand/quiescent)/[rum](https://github.com/tonsky/rum)/[brutha](https://github.com/weavejester/brutha)|
|[Angular $http](https://docs.angularjs.org/api/ng/service/$http)|[cljs-http](https://github.com/r0man/cljs-http)|
|[Angular UI bootstrap](https://angular-ui.github.io/bootstrap/)|[om-bootstrap](https://github.com/racehub/om-bootstrap), [bootstrap-cljs](https://github.com/luxbock/bootstrap-cljs), [re-com](https://github.com/Day8/re-com)|
|[Angular UI router](https://github.com/angular-ui/ui-router)|[secretary](https://github.com/gf3/secretary)|
|[Karma](http://karma-runner.github.io/)|[cljs.test](https://github.com/clojure/clojurescript/wiki/Testing), [doo](https://github.com/bensu/doo)|

Other
-----

|Concept|Clojure|
|-------|-------|
|NoSQL|[monger](http://clojuremongodb.info/), [carmine](https://github.com/ptaoussanis/carmine), [elastisch](http://clojureelasticsearch.info/), [cassaforte](http://clojurecassandra.info/), [alia](https://github.com/mpenet/alia)|
|Storm, Spark|[marceline](https://github.com/yieldbot/marceline), [flamboo](https://github.com/yieldbot/flambo)|
