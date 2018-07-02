---
title: 'Charts from tables'
order: 30
---

## Default graph
Just add ```{: .highchart}``` to the table markdown

| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart}

```
| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart}
```

## Graph type

Custom attributes allows to customize the generated graph. See [Highcharttable plugin documentation](http://highcharttable.org/#doc-graph) for all options.


| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart data-graph-type="spline"}

```
| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart data-graph-type="spline"}
```

---


| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart data-graph-type="area"}

```
| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart data-graph-type="area"}
```

---


| Mois    | Autopano | Panotour |
| ------- | -------- | -------- |
| Janvier | 15       | 7        |
| Février | 25       | 37       |
| Avril   | 55       | 57       |
| Mai     | 45       | 17       |
| Juin    | 48       | 27       |
{: .highchart data-graph-type="line"}


```
| Mois      | Autopano  | Panotour  |
| -         | -         | -         |
| Janvier   | 15        | 7         |
| Février   | 25        | 37        |
| Avril     | 55        | 57        |
| Mai       | 45        | 17        |
| Juin      | 48        | 27        |
{: .highchart data-graph-type="line"}
```

## Options

Custom attributes allows to customize the generated graph. See [Highcharttable plugin documentation](http://highcharttable.org/#doc-graph) for all options.

## Paste from Excel

![paste from excel]({{ "/assets/demo-files/paste-from-excel.gif" | absolute_url }})

1. Copy the data from your spreadsheet
2. Convert the data to markdown, there are many tools available to [convert data sheets to markdown](https://www.google.fr/search?q=excel+table+to+markdown), for example [table generator](https://www.tablesgenerator.com/markdown_tables)
3. Paste the result into your markdown page
