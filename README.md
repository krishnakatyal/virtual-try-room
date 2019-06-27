#  Virtual fitting room

## *This Repository Is Under Construction*
![Sc0379_BoutiqueHotel_116_wg-2](https://user-images.githubusercontent.com/37455387/60255174-d84adf00-98ec-11e9-9286-4ea2aa11ec3d.jpg)

*This virtual dressing room  is the online equivalent of an in-store changing room. It enables shoppers to try on clothes to check one or more of size, fit or style, but virtually rather than physically.*
*A fit technology may be categorised according to the problem that it resolves (size, fit or styling) or according to the technological approach. There are many different types of technological approach.*
*The size of the customer is predicted using Machine Learning :Weight,Size,Gender and Age are the parameters which help in deciding the appropriate fitting.* 
*Real 3D Simulation fitting room combines the features of 3D solutions and photo-accurate fitting rooms. Using both photo and simple body measurements, the solution generates a 3D mannequin, which accurately visualizes customer in chosen apparel items.*

## *Required Software,Hardware And Dependencies Required*:

### *Kinect v2 With Windows Adaptor And Drivers*
 

![Kinect-747x309](https://user-images.githubusercontent.com/37455387/60256293-e26ddd00-98ee-11e9-9f33-b8aa3a488851.jpg)

### *Unity 3D*
![908c28710b023fe94825ed4c503670d9](https://user-images.githubusercontent.com/37455387/60256291-e1d54680-98ee-11e9-98e1-1a8ed4b4e65a.jpeg)

### *OpenCv DLLs*

![OpenCV_Logo](https://user-images.githubusercontent.com/37455387/60256835-efd79700-98ef-11e9-9f4a-6669fac086ba.png)

## *Getting Started*:

### *Settting Up  Kinect And Unity*

*Make sure you have latest sdk browser, drivers and A USB 3.0 Port with which you can connect for Kinect V2,connect the Adaptor to Power source and the other end with Kinect.*
*Download The SDK Browser and the Drivers*
*Select the version of unity you want to install, install Unity hub and visual studio(It gets installed by default)*


### *Fitting Process*
*Fitting process is done by using Iterative closest point (ICP) algorithm to transform the three dimensional model to the joints of human body.*
*In the Iterative Closest Point or, in some sources, the Iterative Corresponding Point, one point cloud (vertex cloud), the reference, or target, is kept fixed, while the other one, the source, is transformed to best match the reference. The algorithm iteratively revises the transformation (combination of translation and rotation) needed to minimize an error metric, usually a distance from the source to the reference point cloud, such as the sum of squared differences between the coordinates of the matched pairs. ICP is one of the widely used algorithms in aligning three dimensional models given an initial guess of the rigid body transformation required*
*The algorithm iteratively revises the transformation (combination of translation and rotation) needed to minimize an error metric, usually a distance from the source to the reference point cloud, such as the sum of squared differences between the coordinates of the matched pairs.*

*Now, to finally place the model on the user's body, the coordinates of ICP transformation are set to the anchors of model.*

*The following 2 transformational components are then set and passed to Unity:*

*Position: The model is placed on the position of body joints*
*Rotation: The model is rotated by an angle equal to the angle made by the joints of human body*


**_[1]Run virtualFittingRoom.exe OR run /Assets/FittingRoom.unity to open it in edit mode._**

**_[2]Stand in front of the Kinect sensor and open your arms as T-Pose to be in control._**

**[3]_The controllers will be moved depending on the movement of your hands_.**

**[4]_Move the controller to select your gender; male/female._**

**[5]_According to your gender a list of clothes and accessories items will be shown in different categories_.**

**[6]_You can select different items from different categories to be fit in your body_.**

**[7]_You can resize the item by clicking on plus and minus button.**

**[8]_You can change the texture of the item by select one of the texture in the textures list.**


## Refernces 
[1]  https://github.com/malakalomari/Virtual-fitting-room

[2] *Kinect-Based Virtual Try-on System: A Case Study by Khalil M. Ahmad Yousef, Bassam J. Mohd, and Malak AL-Omari*
