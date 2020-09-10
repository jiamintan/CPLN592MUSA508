---
title: "Week1"
author: "Jiamin Tan"
date: "September 10, 2020"
output: pdf_document
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

here is my data

```{r mtcars}
str(mtcars)
```

plot the data

```{r plot}
plot(as.factor(mtcars$cyl), mtcars$mpg)
```

and my findings

```{r ttest}
tt <- t.test(mtcars$cyl, mtcars$mpg)
print(tt)
```