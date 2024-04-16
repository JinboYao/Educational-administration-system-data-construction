# Educational-administration-system-data-construction
Construct a unified data warehouse for educational affairs-related data to improve business transparency and optimize the efficiency of educational administration management.

## business process

Analysed user behaviour within the teaching system, sorted out and optimised key business processes including live learning, video learning, course conversion, and assistant teacher and student reach.

![微信截图_20240416204240.png](https://img2.imgtp.com/2024/04/16/8WB1iVUW.png)

## Model

###  model

![微信截图_20240416204323.png](https://img2.imgtp.com/2024/04/16/yJUzC6G1.png)

### latitude matrix

![1713271231579.png](https://img2.imgtp.com/2024/04/16/L48mpQ9f.png)

## Data governance

| Item                | Current Status                                               |
| ------------------- | ------------------------------------------------------------ |
| Data Domain         | pref Performance Domain                                      |
| Data Storage        | Storage: All Education 1.0 data stored as parquet;           |
| Data Quality Issues | ads references ods; The same ods is used in multiple dim/dwd; Logic and indicators are repeatedly constructed, not enough depth; Some tables do not need a long lifecycle (e.g., heartbeat); No dqc except for dim |
| Core Indicators     | Expected attendance, Attendee count, Participant count, Completer count, Number of attendees, Number of participants, Number of completers, Conversion amount in live sessions, Conversion count in live sessions |
| Optimization        | Added business processes and analysis scenarios related to outreach and assignments |
