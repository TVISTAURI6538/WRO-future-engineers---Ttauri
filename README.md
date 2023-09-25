# About-Our-Team-
Mubeen and Vaishant are two young technology enthusiasts who have been working on various coding and robotics projects together for over two years. They both share a passion for innovation and a vision for how technology can make a positive impact in the world. 

Mubeen has a creative mind and natural talent for designing futuristic concepts. He has participated in several competitions related to car design and robotics, and his ambition is to become a robotics engineer. He strives for excellence and thinks about the possibilities of future developments. 
Vaishant's strength lies in coding and programming. He is proficient in over five programming languages and has helped bring Mubeen's designs to life through software. Vaishant provides constructive criticism and feedback that helps them improve their work. His ambition, like Mubeen's, is to work as a robotics engineer. 

Together, Mubeen and Vaishant complement each other's skills and work well as a team. They have gained valuable experience from the small competitions they have participated in so far, and they hope that this is just the beginning of bigger things to come.​
# About-The-Car-

# Electromechanical-Components-




# The-Chassis-

For the chasis we have used a readymade chasis that can support the ackerman's steering mechanism. It is run by a single 12v dc motor.

![chasis measurements](https://probots.co.in/pub/media/catalog/product/cache/d8ddd0f9b0cd008b57085cd218b48832/p/r/probots_metal_smart_racing_platform_for_arduino_raspberry_pi__6.jpeg)

# The-Mecanism-Used-For-Steering-
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
  
# The-Movement-Mechanism- 

The movement of the robot is completely based on a single 12v dc motor. This motor controls the rear axle of the robot using gear's. This gear mechanism was made using 2 
spur gears. One large spur gear and one small gear. The small spur gear is connected to the rear axle of the car, so it is responsible for the rotation of the wheels and the large gear transfers the energy of the motor to the small gear for the wheels to rotate.

![gear mechanism](https://content.instructables.com/FDT/AYT2/J0X5B6CJ/FDTAYT2J0X5B6CJ.png?auto=webp&frame=1&crop=3:2&width=635&fit=bounds&md=bdf7ff456b0fe795c7630e78b1bd723f)

![chasis with motor image](https://content.instructables.com/F3Z/H6RU/J0X5BVQW/F3ZH6RUJ0X5BVQW.jpg?auto=webp&frame=1&width=565&fit=bounds&md=9b89bec24bffbb2222abf1112e99ae92)

![gear pic](https://probots.co.in/pub/media/catalog/product/cache/d8ddd0f9b0cd008b57085cd218b48832/p/r/probots-4wd-chassis-smart-car-s3003-metal-servo.jpeg)

# The-Wheels-

The robot contains high quality rubber wheels with measurements suitable for the robots size and weight. The wheels measurements are also great for the ackerman's mechanism. These wheels also have bearings in them to make their movement smoother.

# Robot-functionality

We have mainly divided the robot's functionality into two main parts, which are :-

  1) Computer Vision 
  2) Environmental Awareness 
  3) Obstacle Avoidance 

1) Computer Vision :-

   The computer vision component of the code is responsible for processing visual information captured by the Raspberry Pi camera module and making navigation decisions 
   based on the detection of specific colors, namely red and green. The process involves the following key steps:

   a) Frame Capture and Color Space Conversion:

        The code continuously captures video frames from the camera, treating each frame as an image.
        These frames are converted from the RGB color space to the HSV (Hue, Saturation, Value) color space. HSV separates color information from brightness and saturation.
  
   b) Color Detection:

        Specific HSV color ranges are defined to identify red and green objects within the frames. These ranges specify the permissible values for hue, saturation, and 
        brightness.

   c) Thresholding:

        After converting to HSV, the code applies thresholding to the frames. This process creates binary masks for red and green, where pixels matching the specified 
        color ranges are highlighted in white, while others are set to black. This binary representation isolates regions where the desired colors are present.

   d) Region of Interest Detection:

        The code identifies regions of interest (ROIs) within the binary masks by detecting connected white regions. ROIs correspond to areas where the red and green 
        colors are detected.

        Bounding rectangles are computed around these ROIs to define their position and size.

   e) Navigation Decisions:

        Based on the positions of these bounding rectangles within the frames, the code makes navigation decisions for the robot.
        If a green marker is within a specific x-coordinate range, the code may command the robot to "turn right."
        If a red marker falls within a certain x-coordinate range, the code may instruct the robot to "turn left."
        If neither color marker is detected within the specified range, the robot may be directed to "stop."

   f) Visual Feedback:

        The code provides visual feedback by annotating the original camera frames with drawn rectangles and lines. These annotations serve to visually indicate the 
        detected color regions and the decision-making process in real-time.

   g) Continuous Operation:

        The entire computer vision pipeline operates within a continuous loop. This loop allows the robot to continually adapt and respond to changes in the positions of 
        the color markers within its environment, enabling real-time color-based navigation.

   
   


   
