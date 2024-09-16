---
title: "Data Quality"
date: 2024-08-15 21:45:00 +0100
categories: [Data Strategy, Data Quality]
tags: [Strategy, Quality, Reading, Synthesis]
---

> **Data Quality** is a critical aspect of *Data Management*, ensuring that considered data is reliable and trustworthy.

## 1. Introduction

Data Quality could be considered as evaluations and checks of your data health. It is a key element to become and stay efficient in decision-making and data operations fields. Whatever the types of data and associated uses we can come accross, taking Data Quality into account right from the start helps maintaining relevant data projects alive.

Evaluating Data Quality is not an easy task, but a few set of metrics and characteristics have emerged over the last few years, giving data practitioners first elements of understanding. Monitoring Data Quality standards through concrete metrics helps tracking changes in Data Quality when data moves (during cleaning, transformation or exploitation operations).

## 2. Data Quality metrics

We often find online a set of various characteristics that define Data Quality, but the most common, agreed and important ones are the following: `Accuracy, Completeness, Consistency, Timeliness, Uniqueness & Validity`.

- **Accuracy** is the ability of data to reflect real-world information in an accurante and reliable way. Coherence of information relative to domain use and trust of data source are key elements to ensure data are accurate.

- **Completeness** is a measure of how complete data is in terms of filled information. The more missing values there are, the more difficult it is to perform analysis, forecasts or even to take appropriate decisions.

- **Consistency** is linked to the coherence of information between multiple data sources and uses. Having trusted and coherent datasets accross various platforms and applications is essential to use data efficiently.

- **Timeliness** is a mean of checking data readiness and the ability to make it available quickly in a desired time frame. This is an important feature to keep users informed data they use are relevant and up-to-date.

- **Uniqueness** the ability to identify in a unique manner records in a dataset. Uniqueness is crucial to avoid errors and ensure aggregations and computations performed during analysis give the right results.

- **Validity** ensures data respect business rules and parameters defined (such as format, values ranges, content expectations, etc.). An invalid dataset should be not used, otherwise at risks of drawing wrong conclusions.

![Data Quality Metrics](assets/2024-08-15-Data-quality/data-quality-metrics.png)

## 3. Concrete examples

Working with Data Quality metrics at first sight can be overwhelming and misleading as scratching the surface of these metrics is often far from sufficient to get results. However, we can go into much details with concrete examples to solve real problems of Data Quality.

With `Accuracy` as a metric to evaluate whether data has no errors and is coherent, it is possible to use **validation rules** or to perform data **profiling methods**. For example, validation rules will help check whether values have errors or inconsistant values (people having negative age, names composed of numbers, birth places not existing, etc.). On the other hand, profiling methods will help with statistical analysis to find the outliers, the incoherent values, the out-of-distribution samples throughout datasets.

`Completeness` really focuses on having data that are filled and complete. **Missing values** analysis, **null values** check and **data imputation** are respectively two metrics and one solution that can be easily implemented in data systems to ensure Completeness. Checking and counting values that are missing or not filled is a really important task to guarantee data can be exploited and brings concrete value later on. Fixing missing values cases with mean/median/mode imputation is a very common pattern to correct this kind of issues.

Data `Consistency` is a critical aspect in distributed systems and large environments, as it states a single data point should be coherent and standardized accross different platforms or systems. **Cross-system checks** and **temporal consistency check** are two possible solutions that can help improving the Consistency metric. Checking whether a single and concrete datapoint is always the same is term of values and meaning accross the various systems is mandatory is guarantee we have consistent data. Performing checks in values, and looking whether values change over time is also important to be sure we have relevant/valuable data.

`Timeliness`, as the capacity to ensure data is up-to-date and ready when needed, can be solved in multiple ways. **Real-time monitoring** of data pipelines and **automated alerts** for delays notification are two possible solutions to face problems with a time dimension. Real-monitoring helps giving information about running data pipelines and their concrete status, to ensure everything is behaving as expected. Automated alerts can be the counterpart of the first solution, to give close-to-real-time information to users and data pipeline managers that something went bad before in the data processing process.

`Uniqueness` is esentially the idea of saying a datapoint can be uniquely identified, and if there is another one likely, it should be the same. **Unicity constraints** and **data matching** are potential solutions to address the Uniqueness metric. Making sure data are organized in tables, with Unicity constraint on the primary keys is one way to be sure there will be no duplicate data. Data matching, whether on full record information, or on a subset of characteristics, can help identify potential duplicates. Fuzzy matching is also possible for more complex issues of Data Quality.

Finally, `Validity` ensures the adherence of considered data with their associated business requirements and standards. **Format checks**, **range checks** and **domain checks** are common rules that can be put in place in order to guarantee the validity of data. Format checks are specific rules on data formats (columns, formats, stored information) with expectations depending on considered information. Range and domain checks are respectively checking rules for numeric values expected to fall in a given range, or values in general to stay coherent with the associated business and domain.

Of course, these are only examples and discussions on what is possible regarding these Data Quality metrics. There are many other ways, methods, and solutions available in the literacy of Data Quality that could be applied.
