# Continuous Intelligence

This site provides documentation for this project.
Use the navigation to explore module-specific materials.

## How-To Guide

Many instructions are common to all our projects.

See
[⭐ **Workflow: Apply Example**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get these projects running on your machine.

## Project Documentation Pages (docs/)

- **Home** - this documentation landing page
- **Project Instructions** - instructions specific to this module
- **Glossary** - project terms and concepts

## Additional Resources

- [Suggested Datasets](https://denisecase.github.io/pro-analytics-02/reference/datasets/cintel/)

## Custom Project

## Dataset

Service provision data for a behavioral health organization. Fields include patient id, date of service, service code and duration in minutes.

## Signals

Duration average calculated to set a baseline to determine threshold from and a column was added to note whether the average exceeded the threshold, returning an anomaly or if it matched the system threshold and would return standard.

## Experiments

Threshold was set at 60 minutes to determine if the average duration surpassed the typically allotted 60 minute timeline.

## Results

Average duration returned at 70, which is above the threshold and outcome column signaled an anomaly.

## Interpretation

The signal and threshold were strict in standards, it's possible settin up a standard deviation and identifying what those are might have added leeway as a set threshold of 60 will likely always return an anomaly. Rolling windows would have deployed successfully with this dataset as well. Having an overall outcome column is helpful in clearly noting what the system identified.
