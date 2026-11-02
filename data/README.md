# Gapminder teaching extract

`gapminder.csv` is a fixed local copy of [Plotly's Gapminder CSV](https://github.com/plotly/datasets/blob/master/gapminderDataFiveYear.csv), retrieved on 2026-11-02. Source file blob SHA: `4ae8fc17a18232b666e4ff8261055007f7dcfaec`.

It contains 1,704 country-year rows: 142 countries observed in 12 five-year steps from 1952 through 2007. It has no missing values in the six supplied columns. It is historical teaching data, not a current global indicator release or complete list of countries.

| Column | Meaning |
|---|---|
| `country` | Country label retained from the source |
| `year` | Observation year |
| `pop` | Population, people |
| `continent` | One of five continent labels used in the extract |
| `lifeExp` | Life expectancy at birth, years |
| `gdpPercap` | GDP per capita, inflation-adjusted US dollars |

Units and scope follow the [Gapminder R package documentation](https://github.com/jennybc/gapminder/blob/main/man/gapminder.Rd). Keep source country and continent labels when reproducing these examples. Do not assume those labels represent every present-day geopolitical boundary.

Each cross-sectional plot filters to 2007. Trend plots connect the same country over time. Means and medians across countries weight each country equally unless explicitly stated otherwise. These summaries are not continental life-table estimates. Repeated observations from a country are not independent people or independent countries.

No dataset download occurs in a revised notebook. To reproduce this snapshot, retrieve the source file at its blob SHA or keep this committed CSV. The file's SHA-256 is `714f8a23e9d7429052a1e9b45d20b9adeb64f46c067ed46320e68182e4607b6d`.

The source repository's MIT notice is reproduced in `PLOTLY_DATASETS_LICENSE.txt`. Original indicator provenance: [Gapminder data](https://www.gapminder.org/data/).
