---
title: 'Forcecoversannotation In Phpunit'
date: 2016-06-08
type: docs
aliases:
  - /projects/til/2016-06-08_forcecoversannotation-in-phpunit/
---
## `forceCoversAnnotation` in PHPUnit

Up until now I've always been using the `beStrictAboutCovers` in the `phpunit.xml` configuration file. Today I learned about the `forceCoversAnnotation` annotation.

The effect is similar: only the code specified by `@covers` will count towards the total code coverage. With `forceCoversAnnotation` however the `@uses` annotation is not required. I like `@uses` but if often clogs up a test class when using lots of small value objects.
