# mermaid 美人鱼

![Header Image](content/images/header.png)

> 用类似markdown的方式从文本来生成图表和流程图
想要简化文档、避免沉重的工具如 Visio 解释代码？
mermaid 美人鱼 就是为此而生，一个简单的 markdown-like 脚本语言，在 javascript 中通过文本来生成图表。 [尝试一下在线编辑器吧][https://mermaidjs.github.io/mermaid-live-editor]


## Request for contribution

- Contribute to mermaid: https://github.com/knsv/mermaid
- Contribute to documentation: https://github.com/mermaidjs/mermaid-gitbook


### An example of a flowchart

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```


### An example of a sequence diagram

```mermaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->John: Hello John, how are you?
    loop Healthcheck
        John->John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->Alice: Great!
    John->Bob: How about you?
    Bob-->John: Jolly good!
```


### An example of a gantt diagram

```mermaid
gantt
        dateFormat  YYYY-MM-DD
        title Adding GANTT diagram functionality to mermaid
        section A section
        Completed task            :done,    des1, 2014-01-06,2014-01-08
        Active task               :active,  des2, 2014-01-09, 3d
        Future task               :         des3, after des2, 5d
        Future task2               :         des4, after des3, 5d
        section Critical tasks
        Completed task in the critical line :crit, done, 2014-01-06,24h
        Implement parser and jison          :crit, done, after des1, 2d
        Create tests for parser             :crit, active, 3d
        Future task in critical line        :crit, 5d
        Create tests for renderer           :2d
        Add to mermaid                      :1d
```

Play with mermaid using this [live editor][live-editor].


## Credits

Many thanks to the [d3](https://d3js.org/) and [dagre-d3](https://github.com/cpettitt/dagre-d3) projects for providing the graphical layout and drawing libraries!
Thanks also to the [js-sequence-diagram](https://bramp.github.io/js-sequence-diagrams) project for usage of the grammar for the sequence diagrams.

*Mermaid was created by Knut Sveidqvist for easier documentation.*

Knut has not done all work by himself, here is the full list of the projects [contributors](https://github.com/knsv/mermaid/graphs/contributors).


# Downstream projects

Mermaid is supported in a number of publishing systems and editors. Please report if a plugin/editor is missing from the list below:

* [Markdown Plus](https://mdp.tylingsoft.com/) - Markdown editor with extra features
* [gitbook-plugin](https://github.com/JozoVilcek/gitbook-plugin-mermaid)
* [Confluence plugin](https://marketplace.atlassian.com/plugins/org.anvard.atlassian.mermaid-plugin/server/overview)
* [Using mermaid via docpad](http://nauvalatmaja.com/2015/01/13/rendering-mermaid-in-docpad/)
* [Using mermaid in Jekyll](https://rubygems.org/gems/jekyll-mermaid/versions/1.0.0)
* [Using mermaid via Octopress](http://mostlyblather.com/blog/2015/05/23/mermaid-jekyll-octopress/)
* [Mardown editor Haroopad](http://pad.haroopress.com/user.html)
* [Plugin for atom](https://atom.io/packages/atom-mermaid)
* [Vim Plugin](https://github.com/kannokanno/previm)
* [Sphinx extension](https://github.com/mgaitan/sphinxcontrib-mermaid)
* [Pandoc filter](https://github.com/raghur/mermaid-filter)
* [hads](https://github.com/sinedied/hads)
* [Mermaid Preview for VS Code](https://marketplace.visualstudio.com/items?itemName=vstirbu.vscode-mermaid-preview)
* [Package for Sublime Text 3](https://packagecontrol.io/packages/Mermaid)


# Online live editor

An editor is available for creating diagrams. With it you can quickly start writing mermaid diagrams. It is possible to:

* save the result as a svg
* get a link to a viewer of the diagram
* get a link to edit of the diagram to share a diagram so that someone else can tweak it and send a new link back

* [Editor][live-editor]

[live-editor]: https://mermaidjs.github.io/mermaid-live-editor/
