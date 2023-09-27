# Our-Team-
Vaishant - responsible for coding and hardware.

Mubeen - responsible for the placement of electromechanical components and chassis structuring.

Mr.Thomas - Coach

Ms.Hemalatha - Team Coordinator

# About-Our-Team-
Mubeen and Vaishant are two young technology enthusiasts who have been working on various coding and robotics projects together for over two years. They both share a passion for innovation and a vision for how technology can make a positive impact on the world.

Mubeen has a creative mind and a natural talent for designing futuristic concepts. He has participated in several competitions related to car design and robotics, and his ambition is to become a robotics engineer. He strives for excellence and thinks about the possibilities of future developments. 
Vaishant's strength lies in coding and programming. He is proficient in over five programming languages and has helped bring Mubeen's designs to life through software. Vaishant provides constructive criticism and feedback that helps them improve their work. His ambition, like Mubeen's, is to work as a robotics engineer. 

Together, Mubeen and Vaishant complement each other's skills and work well as a team. They have gained valuable experience from the small competitions they have participated in so far, and they hope that this is just the beginning of bigger things to come.​

# About-The-Car-

## Electromechanical-Components-

1) 12v dc motor with gears


2) MG996R Servo motor

3) Lipo-battery

4) 




## The-Chassis-

For the chasis we have used a readymade chasis that can support the ackerman's steering mechanism. It is run by a single 12v dc motor.

![chasis measurements](https://probots.co.in/pub/media/catalog/product/cache/d8ddd0f9b0cd008b57085cd218b48832/p/r/probots_metal_smart_racing_platform_for_arduino_raspberry_pi__6.jpeg)

## The-Mechanism-Used-For-Steering-
For the steering system we have used the ackerman's steering mechanism. We chose this because this system had satisfied all our expectations and would work best for our robot. We had researched immensely to find the steering system that would be best for our robot. We had tested multiple steering systems like rack and pinion steering, electronic rear motor steering, 4 wheel steering and hydraulic steering. But all of these mechanisms had many setbacks that would slow down our robot. The perfect mechanism was servo based ackerman's steering. It had great speed and accurate turning even on sharp turn's.

![steering mechanism](https://content.instructables.com/FA5/WOWE/J0X5B80H/FA5WOWEJ0X5B80H.png?auto=webp&frame=1&crop=3:2&fit=bounds&md=297a80991ec822f92a05d6a451b578e0)

![servo attachments](https://content.instructables.com/FN1/ERIB/J0X5B8OX/FN1ERIBJ0X5B8OX.png?auto=webp&frame=1&crop=3:2&width=600&fit=bounds&md=e88b77f274aa201ded7625af0a4e7f3a)

![wheel positioning with mechanism](https://content.instructables.com/FG1/ROSG/J0X5BCST/FG1ROSGJ0X5BCST.png?auto=webp&frame=1&crop=3:2&fit=bounds&md=a65c5b56417a30777fa6017183c3aa85)

![chasis image](https://content.instructables.com/FDU/1WEM/J0X5BMKW/FDU1WEMJ0X5BMKW.jpg?auto=webp&frame=1&width=384&height=1024&fit=bounds&md=2a5c0f83dd895df9d00cbd48b8b6d30f)

![chasis top view](https://content.instructables.com/FME/8EP4/J0X5BMNX/FME8EP4J0X5BMNX.jpg?auto=webp&frame=1&crop=3:2&width=384&height=1024&fit=bounds&md=cba63285974b6d84538d35c6ad2d8a2e)

We had chosen this steering system mainly because of these factors :-

  1) Reduced Tire Wear: Ackermann steering geometry helps reduce tire scrubbing during turns. When a vehicle's wheels follow different turning radii, the tires don't slide 
     sideways (as they would in a non-Ackermann system), leading to less tire wear and longer tire life.

  2) Improved Handling and Stability: Ackermann steering provides better handling and stability during turns. It helps prevent understeer (where the vehicle continues in a 
     straight line despite steering input) and oversteer (where the rear of the vehicle slides out) by ensuring that all wheels follow their intended paths.

  3) Predictable Steering Response: Vehicles equipped with Ackermann steering have a more predictable and consistent steering response. This is especially important in
     high-performance vehicles, where precise control is essential.

  4) Safer Cornering: By reducing the likelihood of tire scrubbing and maintaining better traction during turns, Ackermann steering contributes to safer cornering, 
     especially at higher speeds.

  5) Enhanced Maneuverability: In low-speed maneuvering, such as parking and tight turns, Ackermann steering allows for a smaller turning radius, making the vehicle more 
     maneuverable and easier to handle in confined spaces.

The other steering mechanism lacked in atleast 2 of the above factors, So evidently Ackerman's mechanism was our best choice.
  
## The-Movement-Mechanism- 

The movement of the robot is completely based on a single 12v dc motor. This motor controls the rear axle of the robot using gear's. This gear mechanism was made using 2 
spur gears. One large spur gear and one small gear. The small spur gear is connected to the rear axle of the car, so it is responsible for the rotation of the wheels and the large gear transfers the energy of the motor to the small gear for the wheels to rotate.

![gear mechanism](https://content.instructables.com/FDT/AYT2/J0X5B6CJ/FDTAYT2J0X5B6CJ.png?auto=webp&frame=1&crop=3:2&width=635&fit=bounds&md=bdf7ff456b0fe795c7630e78b1bd723f)

![chasis with motor image](https://content.instructables.com/F3Z/H6RU/J0X5BVQW/F3ZH6RUJ0X5BVQW.jpg?auto=webp&frame=1&width=565&fit=bounds&md=9b89bec24bffbb2222abf1112e99ae92)

![gear pic](https://probots.co.in/pub/media/catalog/product/cache/d8ddd0f9b0cd008b57085cd218b48832/p/r/probots-4wd-chassis-smart-car-s3003-metal-servo.jpeg)

## The-Wheels-

The robot contains high quality rubber wheels with measurements suitable for the robots size and weight. The wheels measurements are also great for the ackerman's mechanism. These wheels also have bearings in them to make their movement smoother.

# Robot-Algorithm-

The robots algorithm is mainly divided into three main parts, which are :-

1) Computer Vision :-

   The Raspberry Pi camera module's visual data is processed by the computer vision part of the algorithm, which also determines where to go depending on the detection of 
   certain colors, especially red and green. The procedure consists of the following crucial steps:

   a) Frame capture and conversion of color spaces:

        Each video frame is treated as an image by the algorithm as it continuously takes video frames from the camera.
        From the RGB color system to the HSV (Hue, Saturation, Value) color space, these frames are converted. Brightness and saturation are dissociated from color 
        information using HSV.
  
   b) Detection of color:

        For the purpose of identifying red and green objects within the frames, specific HSV color ranges are defined. The acceptable hue, saturation, and brightness 
        values are listed in these ranges.

   c)Thresholding:

        The code thresholds the frames after converting them to HSV. Red and green binary masks are created using this procedure, with pixels matching the given color 
        ranges being highlighted in white and the other pixels being set to black. This illustration highlights the areas that have the desired colors.

   d) Identifying a Region of Interest:

        The code finds connected white patches to represent regions of interest (ROIs) within the binary masks. ROIs stand for regions of interest where red and green 
        colors can be seen.

        To determine the location and size of these ROIs, bounding rectangles are computed around them.

   f) Giving Arduino instructions or data:

        The programming directs the robot's navigation based on the locations of these bounding rectangles inside the frames.
   
        The code may command the Arduino to turn the robot right if a red marker is present within a specified x-coordinate range by powering a single pin attached to the 
        Arduino, which is then recognized by the Arduino using the digitalRead function.
   
        The code may direct the Arduino to turn the robot left by powering a single pin that is linked to the Arduino, which is then recognized by the Arduino using the 
        digitalRead function, if a green marker is present within a specific x-coordinate range.
   
        If neither color marker is found inside the designated range, the Arduino is instructed to instruct the robot to keep avoiding obstacles.

   g) Constant Activity:

        the framework of which the entire computer vision pipeline is an ongoing cycle. Real-time color-based navigation is made possible by this loop, which enables the 
        robot to continuously adapt and react to changes in the placements of the color markers inside its environment.

2) Lap Detection:-

   The lap detection in the vehicle is done using a TCS-34725 RGB light col our sensor.
   
   ![TCS 34725 module](https://www.sunrom.com/media/product/299.jpg)

   It is a very accurate and fast colour sensor. It recieves the rgb values of the 
   surface it is used on and based on these values we can decide what shade of red, green or blue the colour of the surface is. As we know, in the RGB reading the red 
   value would be greater than the green and blue values. so if the arduino senses a spike of red in the data recieved from the colour sensor it means the colour detected 
   would be orange with respect to the game field. So using a loop the arduino makes a count of every red spike it detects and when the count reaches to twelve, after a 
   certain time period the program would stop.

3) Obstacle avoidance:-

   The obstacle avoidance is taken care of by the Arduino and 3 ultrasonic sensors, placed in the left, right and the front part of the robot. First the distance is 
   measured from each of these ultrasonic sensors, and the robot simply moves to the side where the distance is maximum. However there is a high chance of error in this 
   algorithm if the speed, turn angles and time is not coordinated. So the robot is well calibrated with predefined values of speed and other factors. The math.h library 
   is used to find the max distance using the max function.

## Conclusion-

This algorithm is based on a single Raspberry Pi and an Arduino MEGA. The Arduino is responsible for the movement and management of all sensors of the robot, while the Raspberry PI is responsible for the processing of the image data recieved from the camera and decision making based on the data recieved. It can also be called as the command centre of the obstacle challenge as it passes commands to the arduino in order for the robot to react to the red and green traffic signs or to continue with the obstacle avoidance.





   
   


   
