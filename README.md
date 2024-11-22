# RAS Config

## Overview
This repository contains the configuration files necessary to set up and customize robot-specific operations for your lab. It includes robot-specific configurations, custom launch files, and lab-specific setup information.

## Contents
- **Custom Launch Files**: These launch files are specific to each robot and are used to tailor their behavior for different scenarios in the lab.
- **Lab Setup Configuration (YAML)**: Contains the configuration of the lab environment, including setup and any specific parameters required for the robots to operate effectively.

## Adding Configurations


### Example YAML Configuration
Here is an example snippet of the container asset YAML configuration:

```yaml
containers:
  - type: beaker
    id: A
    aruco_id: ###
    content_name: empty
    content_volume: 0
    content_color: none
    active_status: 1
    position: [0.5, 0, 0]
    landmark: none
  - type: beaker
    id: B
    aruco_id: ###
    content_name: copper sulphate
    content_volume: 100
    content_color: blue
    active_status: 0
    position: [0.8, 0, 0]
    landmark: none
  - type: test tube
    id: C
    aruco_id: ###
    content_name: empty
    content_volume: 0
    content_color: none
    active_status: 0
    position: [1.2, 0, 0]
    landmark: test-tube rack

```
### Notes
- Ensure that all relevant files have been validated and tested before pushing to the repository.
- If you are working with multiple robots, each launch file should be named clearly to indicate the robot it belongs to.

## Contributing
Feel free to open issues or pull requests if you have suggestions or improvements. Contributions are always welcome!

## License
This project is licensed under the MIT License. See the LICENSE file for more information.

