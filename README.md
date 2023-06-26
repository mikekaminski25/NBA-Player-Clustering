# NBA-Player-Clustering

This was initially my capstone project for my master's in Data Science @ Northwestern.  I graduated a year ago (time flies), so I decided to revisit the code. The goal of this project was to reclassify/recategorize traditional NBA positions (Center, Power Forward, Small Forward, Shooting Guard, Point Guard.  The game of basketball has changed significantly over the years and the traditonal positions might not be the best way to categorize players. 
  * Inception - 1970s: League was dominated by big men
  * 1980s - modern era: Three point shot introduced, less reliance on big men
  * 1990s - 2000s: Shift to defensive minded strategy
  * 2010 - Present: Three point revolution, higher scoring games, faster pace. 
 
The project is now in 3 parts:
1. Clenaing the data
   * This part of the process is relatively unchanged.  The cleaning proess was a bit tedious, but necessary.
   * Data was scraped from the 2000-01 season to the 2021-2022 season
   * There were 4 different stat categories
     + Advanced
     + Per Game
     + Per 100 Possessions
     + Shooting
  * From these, 76 different stats were aggregated and used as features.
  * Insignificant players were removed based on minutes per game and games per season
2.  Analysis
   * This part used tidymodels, which is a package that I've been learning over the past year.
   * This part also further explores the modelings ide.
     + Using PCA to reduce dimensionalty, running multiple PCA iterations of the model.
       + different cutoffs for minutes per game and game played
       + using only variables from each of the 4 stat categories
     + Using K-Means and K-Means w/ PCA
     + Using Hierarchical Clustering
3. Results
  * This is where I've added a ton more visualizations
  * It provides a more in-depth look at each cluster.
