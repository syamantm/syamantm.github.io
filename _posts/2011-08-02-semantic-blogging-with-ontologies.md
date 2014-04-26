---
layout: post-no-feature
title: "Semantic Blogging with Ontologies"
description: "The idea of semantic blogging is to annotate blog contents"
category: articles
tags: [sample post, readability, test]
---

In the previous post I have talked about semantic blogging and it's scopes. In this post I aim to define the concept of semantic blogging more formally and introduce you to some of the ontologies that should be used.

As I have mentioned [earlier](http://blog.syamantakm.com/posts/1-Thoughts-on-Semantic-Blogging) the idea of semantic blogging is to annotate blog contents, i.e. blog posts, comments and tags with ontologies so that the blog metadata can be processed easily by applications and make the reuse of data possible.  One important point to remember is to use already existing and popular ontologies so that the meaning is understood by everyone.  In order to  do that we need to find ontologies that describe the social web  well enough and are popular at the same time. 

SIOC is one such ontology that not only describe the social context but also has gained recognition among the semantic web community. [SICO](http://sioc-project.org/ontology) stands for semantically interlinked online communities and designed by [DERI](http://www.deri.ie/). It defines classes and properties in [OWL](http://www.w3.org/TR/owl-features/) to model relationships within the online communities. Now the question is what are the obvious classes and properties that we can reuse from SIOC ?  One of the classes in it is *sioc:Item* (assuming *sioc* is the namespace used) which can be used to denote a blog post. Similarly *sioc:num_replies* can be used to denote the number of comments for that particular blog post. 

Another important ontology/vocabulary when defining metadata is [Dublin Core](http://dublincore.org/) ontology. Dublin Core has some generic terms that can be useful in the context of the blog as well. For example we can use *dc:title* to denote the title of the blog (assuming we are using *dc* as the namespace). Similarly *dc:created* can be used to denote the post creation time and *dc:modified* to denote last update date. 

The last thing I want to mention is the representation of tags with ontologies. A considerable amount of research is currently going on to find out the best possible solution. It you up to you to decide the level of complexity and therefore the level of richness that you want to achieve in the definition of tags. But either way [SKOS](http://www.w3.org/TR/2008/WD-skos-reference-20080829/skos.html) ontology and [Richard Newman's](http://www.holygoat.co.uk/) ontology for tags are good candidate in this section.

One ontology I haven't mentioned so far is [FOAF](http://www.foaf-project.org/). You can use FOAF to model the users in your blog, e.g. *foaf:name* to denote the name of the user and so on.

Hopefully this should serve as the starting point for you. Do check out the ontologies I have mentioned to find out more and see what classes/properties fits you best.
