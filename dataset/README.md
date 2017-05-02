# Reference datasets

Mafalda framework was used to extract high-level indications starting from a large number of low-level parameters acquired by the car via _OBD-II_ and through the micro-devices embedded in the user smartphone, with the goal of accurately characterizing the overall system composed by driver, vehicle and environment.

A dedicated dataset was collected for the framework evaluation. A subset of the collected data is publicly available here, related to the following cars:

- Peugeot 207 1.4 HDi (70 CV)
- Opel Corsa 1.3 HDi (95 CV) 

Collected data consist of:

- *altitude change*, calculated over 10 seconds;
- *speed*: current value, average and variance in the last 60 seconds and change in speed for every second of detection;
- *longitudinal and vertical acceleration*, measured by the smartphone accelerometer and pre-processed with a low-pass filter to delete high frequency signal components due to electrical noise and external forces;
- *engine load*, expressed as a percentage;
- *engine coolant temperatures*;
- *Manifold Air Pressure* (MAP), a parameter the internal combustion engine uses to compute the optimal air/fuel ratio;
- *Mass Air Flow* (MAF) Rate measured in g/s, used by the engine to set fuel delivery and spark timing;
- *Intake Air Temperature* (IAT) at the engine entrance;
- *Revolutions Per Minute* (RPM) of the engine;
- *average fuel consumption*, calculated as needed liters per 100 km.

Each dataset also contains a label for the following output classes:

- *Road Surface*: Even, Slightly Uneven, Uneven; 
- *Traffic*: Low, Medium, High;
- *Driving Style*: Aggressive, Even Pace.

Data are available both in CSV and [ARFF](http://www.cs.waikato.ac.nz/ml/weka/arff.html "ARFF file format") file format.