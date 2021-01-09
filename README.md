# Spark-Anomaly-Detection

Data: https://www.backblaze.com/blog/backblaze-hard-drive-stats-q1-2019/

Reference: https://www.backblaze.com/b2/hard-drive-test-data.html

INTRODUCTION
Anomaly detection is a technique used to identify unusual patterns that do not
conform to expected behavior, called outliers.
Anomalies can be broadly categorized as:

1. Point anomalies: A single instance of data is anomalous if it’s too far off from the
rest. Business use case: Detecting credit card fraud based on “amount spent.”

2. Contextual anomalies: The abnormality is context specific. This type of anomaly is
common in time-series data. Business use case: Spending $100 on food every day
during the holiday season is normal, but may be odd otherwise.

3. Collective anomalies: A set of data instances collectively helps in detecting
anomalies. Business use case: Someone is trying to copy data form a remote machine
to a local host unexpectedly, an anomaly that would be flagged as a potential cyber
attack.

Given the hard drive logs, implement a point anomaly
detector for:

a) Annualized Failure Rate (by model)

b) Normalized Read Error Rate, SMART attribute 1.

- For generating training labels, use a) 2% b) 100

For an explanation of hard drive SMART attributes, refer to:
https://en.wikipedia.org/wiki/S.M.A.R.T.#Known_ATA_S.M.A.R.T._attributes
