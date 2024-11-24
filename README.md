# HPAwIO_Improved
This dataset has been derived from the original HPAwIO dataset (https://github.com/gokhanmemis/HPAwIO) and migrated to the Apache Parquet format to meet specific requirements. It has been optimized for seamless reading using Pandas. Data related to participants has been consolidated, allowing all processing to be performed on a single file.

Please DO NOT modify this dataset directly.

## Tar & UnTar Information
```bash
tar -czvf - HPAwIO_Improved.parquet | split -b 80M - HPAwIO_Improved.tar.gz

cat HPAwIO_Improved.tar.* | tar -xzvf -
```

# HPAwIO Dataset
HPAwIO is a Physical Activity dataset. This dataset contains mobile phone and oximeter sensors data and labeled with Physical Activity with Indoor and Outdoor information.

# Dataset Information
The recorded dataset contains data from 4 different physical activities and for 2 different locations. All physical activities in the protocol were carried out for about 10 minutes. It was collected more than 16 hours of data using the sensors, labeled as one of 4 different PAs for 2 different locations during data collection. All twelve male and female subjects performed all the activities. In addition, data collection was performed at different times during the day. These hours were from 7 am to 11 am in the morning, from 12 pm to 4 pm in the afternoon, and from 6 pm to 12 am in the evening. This dataset contains 27 features and one class value. Each record consisted of the accelerometer, Gyroscope, Magnetometer, Clinometer, and oximeter signals and was annotated by physical activitie label. All collected records were divided into 3 different age groups, namely Group-A (age between 18 - 34), Group-B (age between 35 - 54), and Group-C (age between 55 - 65). Each subject performed all PAs and we labeled the records with a granularity of 1 millisecond. There are 8 different files consisting of such data, for each subject.

# Dataset Sumary
Labels : Indoor Walking, Outdoor Walking, Indoor Running, Outdoor Running, Indoor Sitting, Outdoor Sitting, Indoor Standing, Outdoor Standing
Feature Count : 27
Number Of Subjects : 12
Number Of Activities : 8
Sensor Placement : Right trouser pocket, right hand, left forefinger
