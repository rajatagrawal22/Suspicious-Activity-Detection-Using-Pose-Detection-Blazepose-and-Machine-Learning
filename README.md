Suspicious activity is a type of behaviour that can be classified as unusual and
may indicate illicit intent. Detecting these types of activities using conventional
methods is a big-time challenge as these methods suffer from computational complexity which limits their real time applicability. This research proposes a machine
learning pose detection framework for identifying suspicious activity. Suspicious
activities involve unusual movements of the body which might be an indication of a
potential threat. By combining pose detection model and classification algorithms
this framework tries to enhance the surveillance systems in real time. The proposed
framework combines a pose estimation model, an activity classification model, an
activity recognition model, and an alert mechanism. The framework proposes to
use MediaPipe BlazePose pose estimation model to extract body posture features
in the form of x, y, and z coordinates. These coordinates are later used to create customised geometric features and train the model. The framework proposes
to create two separate models where the primary model is used to classify if the
activity is suspicious or not and the second model is used to recognize the activity
if predicted as suspicious by the first model. A large-scale dataset of 1900 real
world surveillance videos which consists of 13 different classes is used for this study.
Once the features were extracted from this data four algorithms XgBoost, Random Forest, LightGBM, and Deep Neural Network (DNN) were evaluated for both
primary and secondary models. Random Forest was determined to be the optimal
primary model with an accuracy of 93% and XgBoost was found to be more feasible
as a secondary model with an accuracy of 70% in predicting activities. The potential users who can be benefited from this framework include security companies,
private businesses, public safety organizations, etc. .
