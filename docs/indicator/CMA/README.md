# Cumulative Moving Average

## About

* Added in: [0.1.0](https://github.com/wuhkuh/talib/releases/tag/0.1.0)
* Type: Trend indicator

## Research

### Sources

| Type        | Name                      | By     | Retrieved at | Reference |
| :---------- | :------------------------ | :----- | :----------: | :-------: |
| **Primary** | **Could not be found!**   |        |              |           |
| Tertiary    | Cumulative Moving Average | RTMath |  2017-08-20  | [Reference](https://rtmath.net/helpFinAnalysis/html/f90144b2-8ccb-4eeb-a622-4bd1ff87feb4.htm) |
| Tertiary    | Cumulative Moving Average | QKDB   |  2017-08-21  | [Reference](https://qkdb.wordpress.com/tag/cumulative-moving-average/) |

Sources are ordered by type and trustworthiness.

### Derived formula

![](CMA.png)

To calculate the next CMA, this formula is used:  

![](CMA1.png)

Where `n` is the number of elements and `x` is the current value (usually price).

### Unit tests

<table>
  <tr>
    <th>Input</th>
    <td>17</td>
    <td>23</td>
    <td>44</td>
    <td>12</td>
    <td>2</td>
    <td>36</td>
    <td>37</td>
    <td>44</td>
    <td>28</td>
    <td>20</td>
  </tr>
  <tr>
    <th>Output</th>
    <td>17</td>
    <td>20</td>
    <td>28</td>
    <td>24</td>
    <td>19.6</td>
    <td>22.33333</td>
    <td>24.42857</td>
    <td>26.875</td>
    <td>27</td>
    <td>26.3</td>
  </tr>
  <tr>
    <th><a href=https://qkdb.wordpress.com/tag/cumulative-moving-average/>Reference</a></th>
  </tr>
</table>

## Pseudo-code