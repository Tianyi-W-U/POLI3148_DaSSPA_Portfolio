# Data visualization memo

## Workflow

1. Load the dataset

2. Identify the relevant indicator
3. Select the variable and rename



## Reading Materials on Data Visualization

- [Kabacoff] Kabacoff, Rob. Data Visualization with R. 2020. E-book: [rkabacoff.github.io/datavis](https://rkabacoff.github.io/datavis/)
- [Healy] Healy, Kieran. Data visualization: a practical introduction. Princeton University Press, 2018. E-book: [socviz.co](https://socviz.co/)



## Additional syntax of "+"

```R
# In data wranggling, we use the pipe, like this
d |> select(gdppc)
# In data visualization, aside from the pipe, we also use the "+", like this
d |> # Specify the data frame to plot
  ggplot(aes(x = gdppc, y = life_expectancy)) + # Specify the variables to plot
  geom_point() + # Choose the visualization tool: point
  labs(x = "GDP per capita", y = "Life Expectancy", # set up the axes' titles
       title = "Wealth and Health in the World (1800-2019)", # set up the figure's title
       caption = "By Haohan Chen. Data source: V-Dem v.13") # set up footnote
# It's like a step-by-step painting!
```



## Choose visualization tools

1. Identify the **type** of variable: Continuous or categorical?

2. For continuous:
   1. Summary statistics

### Continuous

#### Summary Statistics

#### Graphs

##### Histogram

##### Density



