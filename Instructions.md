# Homework 03: Use dplyr/ggplot2 to manipulate and explore data
## Overview
Due Tuesday 2018-10-02 at 23:59.

The goal is to manipulate and explore a dataset with the dplyr package, complemented by visualizations made with ggplot2. You can think of this as a deeper version of Homework 02.

Your homework should serve as your own personal cheat sheet in the future for ways to manipulate a dataset and produce companion figures. Give yourself the cheatsheet you deserve! Check out the sampler concept for inspiration.

## Evaluation
All rubrics listed on the assignments page are relevant for this assignment.

For this assignment, you can think of the scores loosely this way:

0: Did not attempt.

1: Didn’t tackle at least 3 tasks. Or didn’t make companion graphs. Didn’t interpret anything but left it all to the “reader”. Or more than one technical problem that is relatively easy to fix. It’s hard to find the report in this crazy repo.

2: Hits all the elements. No obvious mistakes. Pleasant to read. No heroic detective work required. Solid.

3: Exceeded the requirements in number of tasks. Or developed novel tasks that were indeed interesting and “worked”. Impressive use of dplyr and/or ggplot2. Impeccable organization of repo and report. You learned something new from reviewing their work and you’re eager to incorporate it into your work.

## Bring rectangular data in
Work with the gapminder data we explored in class. If you really want to, you can explore a different dataset. Self-assess the suitability of your dataset by reading this issue, and if you still aren’t sure if it’s suitable, send Vincenzo an email.

The Gapminder data is distributed as an R package from CRAN.

# The Assignment
## Your mission, high-level
Pick at least three of the tasks below (in the “Task menu” section) and attack each with a table and figure. For each table, make sure to include a relevant figure! Note that:

dplyr should be your data manipulation tool
ggplot2 should be your visualization tool
Make observations about what your tables/figures show and about the process.

Also useful for you to add to your “cheat sheet” are notes on difficulties/oddities. For example, which figures are easy/hard to make, which data formats make better inputs for plotting functions vs. for human-friendly tables.

If relevant, give credit to your sources, whether it’s a blog post, a fellow student, an online tutorial, etc. This is also valuable “cheat sheet” info for future-you.

## Don’t worry about…
Relax about the following things:

Tidying/reshaping is NOT your assignment. Many of your tables will be awkwardly shaped in the report. That’s OK.
Table beauty is not a big deal. Simply printing to “screen” is fine. You could also try the knitr::kable() function. Assuming my_df is a data.frame, here’s an R chunk that should print it as a decent-looking table:
```{r results = 'asis'}
knitr::kable(my_df)
```
For all things, graphical and tabular, if you’re dissatisfied with a result, discuss the problem, what you’ve tried and move on.
Your figure does not have to depict every single number from the data aggregation result. Use your judgement. It just needs to complement the table, add context, and allow for some sanity checking both ways.

## Task menu
Here are some sample tasks for you to populate your cheat sheet with. If you want to do something comparable but different, i.e. swap one quantitative variable for another, be my guest! If you are feeling inspired and curious, then we’re doing this right. Go for it.

- Get the maximum and minimum of GDP per capita for all continents.

- Look at the spread of GDP per capita within the continents.

- Compute a trimmed mean of life expectancy for different years. Or a weighted mean, weighting by population. Just try something other than the plain vanilla mean.

- How is life expectancy changing over time on different continents?

- Report the absolute and/or relative abundance of countries with low life expectancy over time by continent: Compute some measure of worldwide life expectancy – you decide – a mean or median or some other quantile or perhaps your current age. Then determine how many countries on each continent have a life expectancy less than this benchmark, for each year.

- Find countries with interesting stories. Open-ended and, therefore, hard. Promising but unsuccessful attempts are encouraged. This will generate interesting questions to follow up on in class.

Or, make up your own! Between the dplyr coverage in class and the list above, I think you get the idea.

## But I want to do more!
If you’re particularly keen on levelling up the challenge of this assignment, try these things:

- Layout stretch goal: get table and figure side-by-side. This gist might get you started.
- Table stretch goal: there are some really nice fancy table helper packages. This tweet from @polesasunder will point you toward some R packages you may want to check out (pander, xtable, stargazer).

## Finishing up, and Reflection
Once you’re done the above, go back to UBC canvas, and find the “Homework 03” page.

You’re encouraged to reflect on what was hard/easy, problems you solved, helpful tutorials you read, etc. As usual, put this reflection on your canvas submission.

Please add a link to your homework respository to help out our wonderful TA’s.
