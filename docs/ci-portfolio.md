# Continuous Intelligence Portfolio

Britany Kline

2026-04

This page summarizes my work on Continuous Intelligence projects.

## 1. Professional Project

### Repository Link

<https://github.com/BJean-0905/cintel-01-getting-startedv2>

### Brief Overview of Project Tools and Choices

In this first project, setting up the environment and systems was paramount to get started. This process yielded many hours and time to connect the right set up to match my machine and mirror the directions provided. I made many errors and started over completing a version 2 of this project. I made a minor change to the end of the pipeline executed successfully message. Blessed_be_the_data and confirmed that it successfully ran.

## 2. Anomaly Detection

### Anomaly Detection Repository Link

<https://github.com/BJean-0905/cintel-02-static-anomalies>

### Anomaly Detection Techniques

In this project, anomaly detection is explored by defining thresholds for the dataset. I added a minimum value and a maximum value. In years, minimum was 3, maximum was 18. The minimum height was 36, maximum was 72 in inches. I added a column to identify the output by age grouping. 6&Under, 7-12 and 13&Up.

### Artifacts (Anomaly Detection)

The output data successfully identified the data that fell into both my minimum and maximum thresholds and added the additional column classification by age grouping.

### Anomaly Detection Insights

When setting minimums and maximums, the float you identify will be included as an anomaly. Identified thresholds may have other indicators that analysts can build in to help whoever is reviewing the output data. Grouping by age, for example, in the event further action steps are based on such information.

## 3. Signal Design

### Signal Design Repository Link

<https://github.com/BJean-0905/cintel-03-signal-design>

### Signals

I created an incident reporting dataset for this project. I adjusted the original code to change the error rate to a percentage and then rounded to a whole number. I added a signal for the difference in number of days to identify if the report was submitted greater than 1 day.

### Artifacts (Signal Design)

The output data successfully added a column identifying if the report was submitted late, equaling non compliant outcome, or within the 1 day timeframe, equaling compliant.

### Signal Design Insights

Signals can be very beneficial and dynamic based off multiple aspects of the data. A signal could have been designed to both recognize that a report was also unresolved and past 1 day submission timeframe. This project defined a clearer picture on the difference between anomalies and signals and how both are essential but differing in their purpose. Using my own dataset, akin to real world experience, was very helpful in understanding the focus of the module.

## 4. Rolling Monitoring

### Rolling Monitoring Repository Link

<https://github.com/BJean-0905/cintel-04-rolling-monitoring>

### Rolling Monitoring Techniques

For this dataset, I used the provided dataset using timeseries data. Dataset includes timestamp, request, errors and latency in ms. I used a rolling window of 4, with the original rolling mean for the requests, errors and latency. I added standard deviation was added to the requests and errors in relation to the mean.

### Artifacts (Rolling Monitoring)

The output successfully identified the added standard deviation and adjusted the window size from 3 to 4. Data from the first three rows does not provided the added mean and standard deviation columns, clearly identifying were the designated window begins.

## Rolling Monitoring Insights

In timeseries data, rolling windows would be especially beneficial for using real time data and comparing data to relative timelines. Standard deviation provides an added dimension if the data anomalies and signals need to include a predefined deviation from the mean. Standard deviation also stays relatively small in number variations with numbers that are small to being with. If an error range is between 2-9, as it was in this dataset, the mean variation is larger but the standard deviation has only two returns, 1 and 2. This is impactful in thinking about situations were standard deviation may add to your dataset in both negative and positive ways depending on how much noise you want to capture.

## 5. Drift Detection

### Drift Detection Repository Link

<https://github.com/BJean-0905/cintel-05-drift-detection>

### Drift Detection Techniques

In this project, I compared a reference dataset with a current dataset using the provided datasets. The dataset includes fields for requests, errors, total latency in ms. I rounded the orignal data and took this one step further to remove the .0 after the whole number. Original dataset identified the mean for these fields in both the reference and current datasets along with the mean differential between the two. The drifting flag was also present in the original dataset to identify drift between the two defining true/false output. I added the drift detection column to identify if drift was drifting upward, no drift or downward.

### Artifacts (Drift Detection)

The output data successfully added the drift direction columns showing no drift, and upward drift between the reference and current datasets.

### Drift Detection Insights

Drift detection is applicable to numerous types of datasets in comparison to how systems function historically versus real time information. Added value is what direction that drift is heading in. The analyst can see the numbers and compare them but the versality of this clear output would help in many capacities of sharing the output of the drift with audiences. Clear output translates better for a wider variety of audiences.

## 6. Continuous Intelligence Pipeline

### Continuous Intelligence Pipeline Repository Link

<https://github.com/BJean-0905/cintel-06-continuous-intelligence>

### CI Pipeline Techniques

The dataset includes the fields from a made up datset of servision provision in a clinical setting. Fields include patient id, date of service, service code and duration in minutes. Max threshold was set for 60 minutes. Signal was set to identify the average duration. I added a column to designate the state of the duration. Standard vs. anomaly.

### Artifacts (Continuous Intelligence Pipeline)

Output data identified the average duration calculated and if that average was standard or, in this case, an anomaly.

### Assessment

In reflection, I'd like to have added dimensions to this pipeline to allow for variation. Using standard deviation might have been a good decision and then designating a threshold such as 3+ standard deviations from the mean. Systems will always have variation in them, the challenge is finding how much room to allow them to operate within based on numerous factors. I do believe it was beneficial to again, classify the finding. In this case, the system is noted as having an anomaly or finding that needs attention. Clear outcomes are greatly needed in sharing information, especially with those who do not "work behind the scenes".
