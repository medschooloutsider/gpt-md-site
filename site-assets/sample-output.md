# Epidemiology and Biostatistics Study Export

## Dataset setup

The diabetes dataset loaded correctly. The main issue was column-name mismatch.

R is case-sensitive:

- `patients$Age` works
- `patients$age` does not work
- `patients$BMI` works
- `patients$bmi` does not work

The diabetes-status variable is `Outcome`, not `diabetes`.

## Corrected inspection code

```r
nrow(patients)
ncol(patients)
names(patients)
str(patients)
head(patients)
```

## Descriptive statistics

```r
mean(patients$Age, na.rm = TRUE)
median(patients$BMI, na.rm = TRUE)
max(patients$Glucose, na.rm = TRUE)
min(patients$BloodPressure, na.rm = TRUE)
range(patients$BMI, na.rm = TRUE)
quantile(patients$BMI, 0.25, na.rm = TRUE)
```

## Group summaries

```r
table(patients$Outcome)
sum(patients$Outcome == 1, na.rm = TRUE)
tapply(patients$BMI, patients$Outcome, mean, na.rm = TRUE)
tapply(patients$Age, patients$Outcome, mean, na.rm = TRUE)
```

In this dataset:

- `Outcome = 0` means non-diabetic
- `Outcome = 1` means diabetic

## Correlation and plots

```r
cor(patients$BMI, patients$Glucose, use = "complete.obs")
plot(patients$BMI, patients$Glucose)
hist(patients$Age)
boxplot(BMI ~ Outcome, data = patients)
```

Correlation describes association, not causation. A scatterplot should be checked alongside the correlation value.

## Missing values

Some variables may contain values that are missing or biologically implausible.

High-yield commands:

```r
is.na(x)
sum(is.na(x))
which(is.na(x))
mean(x, na.rm = TRUE)
na.omit(dataframe)
```

Example workflow:

```r
sum(is.na(patients$BMI))
which(is.na(patients$BMI))
mean(patients$BMI, na.rm = TRUE)
patients_clean <- na.omit(patients)
mean(patients_clean$BMI)
```

## Week 7 concepts

This section moves from descriptive statistics toward inferential statistics:

- missing values
- normal distribution
- chi-square distribution
- confidence intervals
- hypothesis logic

## Study checklist

By the end of this block, you should be able to:

- import a dataset
- inspect rows, columns, names, and types
- compute descriptive statistics
- interpret correlations
- make scatterplots, histograms, and boxplots
- detect missing values
- ignore or remove missing data appropriately
- explain why distributions matter
- describe the basic logic of hypothesis testing
