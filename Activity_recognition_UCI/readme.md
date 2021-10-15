This dataset contains the motion data of 14 healthy older aged between 66 and 86 years old, performed broadly scripted activities using a batteryless, wearable sensor on top of their clothing at sternum level. Data is sparse and noisy due to the use of a passive sensor.
Participants were allocated in two clinical room settings (S1 and S2). The setting of S1 (Room1) uses 4 RFID reader antennas around the room (one on ceiling level, and 3 on wall level) for the collection of data, whereas the room setting S2 (Room2) uses 3 RFID reader antennas (two at ceiling level and one at wall level) for the collection of motion data.
The activities performed were:
walking to the chair,
sitting on the chair,
getting off the chair,
walking to bed,
lying on bed,
getting off the bed and
walking to the door.
Hence the possible class labels assigned for every sensor observation are:
- Sitting on bed
- Sitting on chair
- Lying on bed
- Ambulating, where ambulating includes standing, walking around the room.

I applied SVM and used k-fold cross validation. Through this notebook I utilized numpy, pandas, and sckit-learn libraries.



#Results:

accuracy is: 0.9311006196518147
precision array([0.36564626, 0.3       , 0.96210297, 0.11764706]) 
recall array([0.46637744, 0.05769231, 0.97115309, 0.04615385])
F1   array([0.4099142 , 0.09677419, 0.96660685, 0.06629834])
