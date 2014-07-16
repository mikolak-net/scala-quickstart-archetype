scala-quickstart-archetype
==========================

Basic Scala archetype.

Usage
=====

The archetype is under development right now. See the [issues list](https://github.com/mikkoz/scala-quickstart-archetype/issues) for details on planned features.

Why yet another archetype?
==========================

An excellent question! First of all, archetypes are sometimes quite underrated as a concept - they provide a gateway to various technologies and frameworks to coders who are not Maven, er, [mavens](https://en.wikipedia.org/wiki/Maven).

Given that, let's take a look at some "generic" archetypes such as `net.alchim31.maven:scala-archetype-simple` or `org.apache.maven.archetypes:maven-archetype-quickstart`. After project creation, it becomes apparent that they serve mainly the following purposes:
* creating the POM boilerplate for the specific project type,
* introducing the POM creator to some associated frameworks, technologies and/or patterns (e.g. the Scala archetype includes no less than **three** different test libraries at the same time).

At this point, coupled with the premise that POMs are essentially executable (declarative) build configuration code, it can be argued that the abovementioned archetypes fail the [SRP](https://en.wikipedia.org/wiki/Single_responsibility_principle).

The archetype you're now viewing, and [its sister project](https://github.com/mikkoz/java8-quickstart-archetype), attempt to alievate this problem.

Namely, they have a single goal in mind: enable a user to create multiple projects, with the most popular *exclusive* configuration *variants*, and with the *least* "educto-boilerplate" to clean up.

The last subpoint emphasises why this goal was chosen as a primary one, over educating newcomers. 

Nowadays, various 3rd party ecosystem libs (such as the aforementioned [three](http://junit.org/) [testing](http://www.scalatest.org/) [libraries](https://etorreborre.github.io/specs2/) ) tend to do a decent job at introducing new developers. Therefore, it is posited that it's more efficient for any given archetype user to have a *tabula rasa* available anytime than to being educated - a job that's somewhat redundant, given the context.
