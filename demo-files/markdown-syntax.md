---
title: 'Markdown syntax'
order: 10
---
## Why Markdown?
> Un document balisé par Markdown peut être lu en l'état sans donner l’impression d'avoir été balisé ou formaté par des instructions particulières.

**Markdown** is a [lightweight markup language](https://en.wikipedia.org/wiki/Lightweight_markup_language) with plain text formatting syntax. It is designed so that it can be converted to [HTML](https://en.wikipedia.org/wiki/HTML) and many other formats using a tool by the same name. Markdown is often used to format readme files], for writing messages in online discussion forums, and to create [rich text](https://en.wikipedia.org/wiki/README) using a [plain text](https://en.wikipedia.org/wiki/Plain_text) editor.

## What is Jekyll?

> Transform your plain text into static websites and blogs.

[Jekyll website](https://jekyllrb.com/) is the [GitHub Pages](https://pages.github.com/) engine and it can be run from your machine.

# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading

```
# h1 Heading
## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading

```



## Horizontal Rules

___

---

***

```
___

---

***
```


## Emphasis

**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Strikethrough~~

```
**This is bold text**

__This is bold text__

*This is italic text*

_This is italic text_

~~Strikethrough~~
```


## Blockquotes

> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.

```
> Blockquotes can also be nested...
>> ...by using additional greater-than signs right next to each other...
> > > ...or with spaces between arrows.
```


## Lists

Unordered

+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!

```
+ Create a list by starting a line with `+`, `-`, or `*`
+ Sub-lists are made by indenting 2 spaces:
  - Marker character change forces new list start:
    * Ac tristique libero volutpat at
    + Facilisis in pretium nisl aliquet
    - Nulla volutpat aliquam velit
+ Very easy!
```

Ordered

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
    1. You can use sequential numbers...
    1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar

```
1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
    1. You can use sequential numbers...
    1. ...or keep all the numbers as `1.`

Start numbering with offset:

57. foo
1. bar
```


## Code

Inline `code`

Indented code

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code


Block code "fences"

```
Sample text here...
```

Syntax highlighting

``` js
var foo = function (bar) {
  return bar++;
};

console.log(foo(5));
```

## Tables

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

```
| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```

Right aligned columns

| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

```
| Option | Description |
| ------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |
```


| Tables        | Are           | Cool  |
|---------------|---------------|------:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```
| Tables        | Are           | Cool  |
|---------------|---------------|------:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```

## External links

This template detects external links and adds an icon ![external link icon]({{ "/assets/demo-files/external-link.svg" | absolute_url }})

[link text](http://dev.nodeca.com)

[link with tooltip](http://nodeca.github.io/pica/demo/ "title text!")

```
[link text](http://dev.nodeca.com)

[link with tooltip](http://nodeca.github.io/pica/demo/ "title text!")
```

## Internal links

Jekyll allows to insert dynamic internal links that work even if the permalink of target pages is set.

[Link to another md file]({{ site.url }}{{ site.baseurl }}{% link demo-files/charts.md %})

```
{% raw %}
[Link to another md file]({{ site.url }}{{ site.baseurl }}{% link demo-files/charts.md %})
{% endraw %}
```

If you change the permalink of these target pages, the build takes it into account and includes the proper link.

## External images

![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

```
![Minion](https://octodex.github.com/images/minion.png)
![Stormtroopocat](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")
```

Like links, Images also have a footnote style syntax

![Alt text][id]

```
![Alt text][id]
```

With a reference later in the document defining the URL location:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"

```
[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"
```

## Local images

With absolute URL

![Le Monal]({{ "/assets/monal.jpg" | absolute_url }})

```
{%raw%}
![Le Monal]({{ "/assets/monal.jpg" | absolute_url }})
{%endraw%}
```

With relative URL, image in the same folder as md file

![External link](search.svg)

```
![External link](external-link.svg)
```

With relative URL, path relative

![External link](../assets/demo-files/external-link.svg)

```
![External link](../assets/demo-files/external-link.svg)
```
