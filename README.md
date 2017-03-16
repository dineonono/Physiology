

title: "Assignment 1"
author: "Dineo Nono"
date: "21 February 2017"
output: md_document


##Hello Octocat
I love Octocat. She's the coolest cat in town.
![](https://dl.dropboxusercontent.com/u/11805474/painblogr/biostats/assignments/octocat.png)
```{r quick_look, echo=TRUE}
data("anscombe")
dim.data.frame(anscombe)
colnames(anscombe)
head(anscombe)
tail(anscombe)
summary(anscombe)

```
```{r xy_plot, echo=FALSE, fig.height=8, fig.width=8, fig.align='center', dev='svg', fig.path= './figures/'}
data("anscombe")
anscombe
with(anscombe, plot(x1, y1))
abline(lm(y1 ~ x1, data = anscombe))
```




