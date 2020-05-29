DC Exercises: Chapters 1 & 2 Solutions
================
by Emily Strong
May 29, 2020

# Exercise 1.1

Recall that a quantitative variable takes on a numerical value, and a
categorical variable tells which category or group a case falls into.

## Part (a)

`Taffy` is the value of a variable for a particular case.

## Part (b)

`year` is a quantitative variable.

## Part (c)

`sex` is a categorical variable.

## Part (d)

`name` is a categorical variable.

## Part (e)

`count` is a quantitative variable.

# Exercise 1.2

Recall that the two rules for tidy data are (1) that the rows (cases)
each refer to a specific, unique and similar unit of observation; and
(2) the columns (variables) each refer to a specific attribute, feature
or measurement of the cases.

Rule (1) for tidy data is violated, because each row in this table
combines several observations across multiple years. Furthermore, the
number of states variable is neither quantitative nor categorical, since
it contains measurements of both types, and so the variable “number of
states” does not use similar units of observation. Finally, the data are
not all in the same format, specifically in the first column. Here is an
example of how the table could be rewritten in tidy form:

<table>

<thead>

<tr>

<th style="text-align:left;">

President

</th>

<th style="text-align:right;">

Office

</th>

<th style="text-align:right;">

States

</th>

</tr>

</thead>

<tbody>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1791

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1792

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1793

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1794

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1795

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1796

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1797

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1798

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

George Washington

</td>

<td style="text-align:right;">

1799

</td>

<td style="text-align:right;">

16

</td>

</tr>

<tr>

<td style="text-align:left;">

Martin Van Buren

</td>

<td style="text-align:right;">

1837

</td>

<td style="text-align:right;">

26

</td>

</tr>

<tr>

<td style="text-align:left;">

Martin Van Buren

</td>

<td style="text-align:right;">

1838

</td>

<td style="text-align:right;">

26

</td>

</tr>

<tr>

<td style="text-align:left;">

Martin Van Buren

</td>

<td style="text-align:right;">

1839

</td>

<td style="text-align:right;">

26

</td>

</tr>

<tr>

<td style="text-align:left;">

Martin Van Buren

</td>

<td style="text-align:right;">

1840

</td>

<td style="text-align:right;">

26

</td>

</tr>

<tr>

<td style="text-align:left;">

Martin Van Buren

</td>

<td style="text-align:right;">

1841

</td>

<td style="text-align:right;">

26

</td>

</tr>

<tr>

<td style="text-align:left;">

Abraham Lincoln

</td>

<td style="text-align:right;">

1861

</td>

<td style="text-align:right;">

34

</td>

</tr>

<tr>

<td style="text-align:left;">

Abraham Lincoln

</td>

<td style="text-align:right;">

1862

</td>

<td style="text-align:right;">

34

</td>

</tr>

<tr>

<td style="text-align:left;">

Abraham Lincoln

</td>

<td style="text-align:right;">

1863

</td>

<td style="text-align:right;">

34

</td>

</tr>

<tr>

<td style="text-align:left;">

Abraham Lincoln

</td>

<td style="text-align:right;">

1864

</td>

<td style="text-align:right;">

34

</td>

</tr>

<tr>

<td style="text-align:left;">

Abraham Lincoln

</td>

<td style="text-align:right;">

1865

</td>

<td style="text-align:right;">

34

</td>

</tr>

</tbody>

</table>

Now, each case is a president in a given year. The variables are
president, year of office, and number of states.

# Exercise 1.3

Recall that variables are quantities that vary from one case to another.

## Part (a)

The variables in Data Table A are `Year`, `Algeria`, `Brazil` and
`Columbia`.

The variables in Data Table B are `Country`, `Y2000` and `Y2001`.

The variables in Data Table C are `Year`, `Country` and `Value`.

## Part (b)

The meaning of a case in Data Table A is a year.

The meaning of a case in Data Table B is a country.

The meaning of a case in Data Table C is a country in a year.

# Exercise 1.5

Recall that the rows (cases) must each refer to a specific, unique and
similar unit of observation, and that each row-case must appear once and
only once in tidy data.

## Part (a)

`sex`,`age` and `gun` time are not part of the meaning of a row-case,
because these variables are attributes or qualities of each case; they
are not units of observation.

## Part (b)

Additional data such as nationality, experience, date of birth, height,
or weight may be used to distinguish between the two Jane Pooles.

# Exercise 2.1

``` r
# install.packages("babynames")
# install.packages("dplyr")
# library(babynames)
baby_data <- dplyr::sample_n(babynames, size=10, replace=TRUE)
```

The preceding example of a command incorporates the following concepts:

  - object name: `baby_data`

  - assignment operator: `<-`

  - package: `dplyr`

  - function: `sample_n`

  - object/data table: `babynames`

  - named argument: `size=10`; `replace=TRUE`

# Exercise 2.3

``` r
?mosaicData::CPS85
# or
library(mosaicData)
?CPS85
# or
library(mosaicData)
help(CPS85)
```

The “Description” section in the documentation for the `mosaicData`
package says that CPS stands for current population survey.

# Exercise 2.5

``` r
?library
# or
help(library)
```

## Part (a)

The “Usage” section in the documentation shows that the function
`require()` has similar arguments to `library()`.

## Part (b)

`search()` is the function after `detach` in the “See Also” section of
the documentation for `library()`.

# Exercise 2.6

The legitimate object names are

  - essay14

  - third\_essay

  - functionList

  - FuNcTiOnLiSt

  - .MyData.

The others are not legitimate object names for the following reasons:

  - `first-essay`: has punctuation in it that is not a period or
    underscore.

  - `"MyData"`: quotes may not be used with object names; they are meant
    to denote character strings.

  - `small sample`: object names must not included spaces.

  - `sqrt()`: this is a function, and also includes punctuation that is
    not a period or an underscore.

# Exercise 2.7

``` r
library(nycflights13)
data(flights)
help(flights)
View(flights)
```

## Part (a)

There are 19 variables; each column in the flights data is a different
variable, because it is a characteristic of one of the flights leaving
NYC.

## Part (b)

There are 336,776 cases.

## Part (c)

The meaning of a case is a flight that departed NYC in 2013.

## Part (d)

The quantitative variables are

  - `year`

  - `month`

  - `day`

  - `dep_time`

  - `arr_time`

  - `sched_dep_time`

  - `sched_arr_time`

  - `dep_delay`

  - `arr_delay`

  - `flight`

  - `air_time`

  - `distance`

  - `hour`

  - `minute`

  - `time_hour`

The categorial variables are

  - `carrier`

  - `tailnum`

  - `origin`

  - `dest`

## Part (e)

The units of `air_time` are minutes. The units of `distance` are miles.

cd username.github.io

echo “Hello World” \> index.html
