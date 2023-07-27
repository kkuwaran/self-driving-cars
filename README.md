# self-driving-cars
This is a software for self-driving cars (based on CARLA Simulator).
- Course1FinalProject: Implement longitudinal and lateral controllers to control the vehicle to follow a race track by navigating through preset waypoints where the vehicle needs to reach at certain desired speeds.
  - Waypoints: "racetrack_waypoints.txt" file
  - Controllers: "controller2d.py" file
    - Longitudinal Controller: PID controller outputting vehicle throttle and brake (in percentage)
    - Lateral Controller: Stanley controller outputting vehicle steering (in radians)
- Course2FinalProject: Implement the Error-State Extended Kalman Filter (ES-EKF) to localize a vehicle using data from the CARLA simulator. The filter relies on IMU data to propagate the state forward in time, and GPS and LIDAR position updates to correct the state estimate.
  - ES-EKF Implementation: "es_ekf.py" file
  - Helping Functions: "rotations.py" file
- Course3Assignment: Implement visual odometry to estimate an autonomous vehicle trajectory by images taken with a monocular camera set up on the vehicle: Extract features from the photographs taken with a camera setup on the vehicle, Use the extracted features to find matches between the features in different photographs, Use the found matches to estimate the camera motion between subsequent photographs, Use the estimated camera motion to build the vehicle trajectory
  - Visual Odometry for Localization in Autonomous Driving: "Visual Odometry for Localization in Autonomous Driving.ipynb" file
  - DatasetHandler (class): "m2bk.py" file
  - RGB images and Depth frames: "data" folder
- Course3FinalProject: Implement a baseline environmental perception stack to extract useful scene information to allow self-driving cars to safely and reliably traverse their environment: Use the output of semantic segmentation neural networks to implement drivable space estimation in 3D, Use the output of semantic segmentation neural networks to implement lane estimation, Use the output of semantic segmentation to filter errors in the output of 2D object detectors, Use the filtered 2D object detection results to determine how far obstacles are from the self-driving car
  - Environment Perception For Self-Driving Cars: "Environment Perception For Self-Driving Cars - Learner - v1.ipynb" file
  - DatasetHandler (class), compute_plane (function), dist_to_plane (function), get_slope_intecept (function), extrapolate_lines (function), find_closest_lines (function): "m6bk.py" file
  - Depth images, RGB images, Segmentation images: "data" folder
  - Output: "images" folder 
