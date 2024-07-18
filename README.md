# Motor_AI_exercise
This is the code and the solution for the exercises for Motor_AI

**Exercise 2**

**b)** Raster masks with similar pixel values were loaded into an ML pipeline but the process broke down before the
training could commence. Which feature(s) were likely to be the culprit(s)? Give reasons for your answer and provide a
solution to this.

**Solution:** There might be many reasons for the breakdown. Some of them are listed below.
a) Pixel values are overlapping.
b) Noise in raster mask can also confuse the machine learning model and hence lead to breakdown.
c) Environmental changes can affect the models ability to generalize as well.
d) class imbalance-If in a dataset there are more pixels representing buildings then it is possible that model will predominantly classify buildings, ignoring roads.
e) If the data is corrupted that prevents the pipeline even from initiating the training process.

**Solutions for breakdown:**
a) Assign distinct and non_overlapping pixels for each class.
b) Either set a specific value to the null values or you can also interpolate.
c) Maybe train the model with imagery from different seasons.
d) Assign hig values to minority classes in loss function.
e) Ensure files can be loaded without errors.




