---
layout: post
title: "Visualizing feature size and dependencies between development teams"
---

When I plan a next major development release, i usally follow an iterative approach, starting with a small workshop where representatives of all teams participate. I use this opportunity to give an overview on the desired features for the upcoming release. In a second step I would ask the teams to give a first judgement on their impact on the presented features. For this i typically use a stripped down QFD matrix (Quality Function Deployment), where all the features are listed in the first column and all the teams are listed in the first row. Going from feature to feature the teams give feedback if they need to contribute for this feature and if yes how big their contribution is. Depending on the granularity of your features and various other factors, the metrics for judging the team contribution might vary. In the example below, the metrics is percentage of available development time until planned release date. But other metrics like,

* Teamweeks
* Storypoints
* 1: low impact - 10: high impact
* ...

are also fine, depending on the results you want to achieve.

![QFD matrix](../../../assets/QFD.JPG)

I normally don't use those results as a valid basis for planning, but rather as a jump of point for answering the following questions:

1. Which features are big and need further scoping?
2. Which features have many participating teams and are therefore risky?
3. Is the overall scope managable or should features be removed for the next release?
4. Are teams underutilized and is there room for additional features?

Although the QFD matrix is great for collecting this data, it is not so good in answering the above mentioned questions, especially when there are a lot of features and development teams involved.
To cope with this draw back, i started experimenting with visualizing the data in different ways.
The Sankey diagram below, shows the most promising results so far. On the left hand side of the diagram all the features are listed and on the right hand side all the development teams. Each line between feature and team represents a contribution of team to this feature and the strenght of the line represents the size of their contribution.
The diagram gives very good insights in answering the questions 1., 2. and 4.


<!--<iframe width="100%" height="935" frameborder="0" src="https://observablehq.com/embed/@d3/parallel-sets?cells=chart"></iframe>-->
<iframe width="100%" height="935" frameborder="0"
  src="https://observablehq.com/embed/687a56d07528b727?cells=test"></iframe>
