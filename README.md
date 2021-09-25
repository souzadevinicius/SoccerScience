# SoccerScience

The project consists of some data science exercises using soccer data.
First of all, I've collected data from the last 14 years Brasileirão Série A and 2. 
## Brazilian 1st division historical data

An example 2015' season's Brazilian 1st division standing.

```R
    Pos Team             Final Points Goals For Goals Against Goals Difference  Year
  <int> <chr>                   <dbl>     <int>         <int>            <int> <int>
1     1 Corinthians                81        71            31               40  2015
2     2 Atlético Mineiro           69        65            47               18  2015
3     3 Grêmio                     68        52            32               20  2015
4     4 São Paulo                  62        53            47                6  2015
5     5 Internacional              60        39            38                1  2015
6     6 Sport Recife               59        53            38               15  2015
```


## Most titles in the period

The data contains data from 2008's to 2021's season.

```R
  Team       Number of Titles
  <chr>          <int>
1 Corinthians        3
2 Flamengo           3
3 Cruzeiro           2
4 Fluminense         2
5 Palmeiras          2
6 São Paulo          1
```
## Number of rounds as a leader in the period

```R
  Team                Rounds
  <chr>               <int>
1 Corinthians           114
2 Flamengo              114
3 Cruzeiro               76
4 Fluminense             76
5 Palmeiras              76
6 São Paulo              38
7 Atlético Mineiro       20
```

## Teams performances in time-series

The figure below shows the overall performance among all teams that have appeared on a brasileirão série at least one time. The blue line shows the home performance. The red-filled line marks the team performance as a visitor.


  - Yellow rectangle marks the champion team
  - Green rectangle marks the Libertadores' zone
  - Black rectangle marks the relegation zone
  - Red rectangle marks the COVID-19 period


![Points Evolution](./plots/performance.png)

## Analysis of a specific season

### Positions throughout rounds

This plot shows the evolution points throughout the rounds among all teams.

First, I've tidy data in this format.

```R
    pos round team        sum_point
  <int> <int> <chr>           <dbl>
1     1     1 Corinthians         3
2     1     2 Corinthians         6
3     1     3 Corinthians         7
4     1     4 Corinthians         7
5     1     5 Corinthians         7
6     1     6 Corinthians        10
```

![Points Evolution](./plots/evolution_points.png)



