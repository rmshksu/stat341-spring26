---
layout: page
title: Practice Data
description: Listing of recommended datasets.
nav_order: 6
---

All of the data used for this class can be found below. This code can be placed into R environment to prepare it as a usable data object. The raw url link can be used in general to access the data.

- Chronic wasting disease

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/CWD_extended.csv"
cwd_extended = read.csv(url, stringsAsFactors = FALSE)
```

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/CWD_land.csv"
cwd_land = read.csv(url, stringsAsFactors = FALSE)
```

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/CWD_simple.csv"
cwd_simple = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Global temperatures

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/GlobalLandTemperaturesByState.csv"
land_temp_state = read.csv(url, stringsAsFactors = FALSE)
```

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/GlobalTemperatures.csv"
globe_temp = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Kansas water level

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/KS_Water_Level_Monitoring_95to13.csv"
ks_water_lev = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Aquatroph experimental

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/aqua_troph_experiment.csv"
aqua_troph = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Coyote scat diet compositions

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/coyote_diet.csv"
coyote = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- CDC Vessel Sanitation Program (Norovirus vigilance)

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/cruisedata.csv"
cruise = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Framingham heart study

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/framingham_heart_study.csv"
framingham = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- Heart biometrics

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/heart.csv"
heart = read.csv(url, stringsAsFactors = FALSE)
```

<br>

- NOAA Tsunami and Earthquake tracking

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/refs/heads/main/tsunami.tsv"
tsunami = (read.delim(url, sep = "\t")[-1,])[,-1]
```

<br>

- Schizophrenic subject reaction times

```
url = "https://raw.githubusercontent.com/rmshksu/teaching-data/4c51b2017bb69c11d7ee918cac7d594c07b39549/schiz.txt"
schiz = data.frame(time = scan(url,skip=5),
                   schizophrenia = c(rep("no",30*11),rep("yes",30*6)))
```