# SimMining-3D
The study proposes a novel approach that addresses the domain shift between synthetic and real data in 3D object detection for complex mining environments. 

![fig1_old](https://github.com/MehalaBala/SimMining_3D/assets/141080983/42679d13-30f4-4b25-80ed-a73bb4e5b9b7)


## Data Collection at simulated environment

The data collection process took place within a representative simulation environment based on the Yandicoogina mine site at Western Australia, as descirbed in cited paper, mirroring real conditions and spanning 583m in longitude and 379m in latitude. The environment's 63.5m elevation provides a comprehensive depiction of the terrain. Earthmoving equipment and sensors were integrated into Gazebo's CAD models.
The dataset's point clouds were obtained using a simulated MST system [reference ours], comprising a 128-line OS2 LiDAR sensor and an RGB camera. The LiDAR sensor captures up to 700,000 points per second with a vertical field of view of 22.5°, boasting an accuracy of ±2.5 to 8 cm. 
The setup included placing the trailer equipped with the sensor both within the mine bench and on higher benches. This allowed for observations of excavators within the pit and on benches exceeding 10 meters in height.

## Data Layout
The dataset encompasses the following information:

**Frames:** This section comprises ply files of point clouds captured from different sensor positions.

**Labels_objectdetection:** Here, you'll find txt label files corresponding to the frames. Each text file contains 3D bounding box information for the excavators in LiDAR coordinates. This information includes the box's center (x, y, and z), dimensions (dx, dy, and dz), yaw value, difficulty level, and object class name. The objects' difficulties are labeled as 0 for easy, 1 for moderate, and 2 for hard.

**Labels_segmentation:** This segment provides pointwise class labels for each scene.

**ros_gtdatabase_hitachi:** Within this section, you'll discover cropped point data of the objects from the scene.

### Download
(https://unisyd-my.sharepoint.com/:f:/g/personal/mehala_balamurali_sydney_edu_au/Enns61uDsTxKjCiiPM4hx9MBizoIc_T4PoeI054PmTPzzA?e=FLo13r](https://unisyd-my.sharepoint.com/personal/mehala_balamurali_sydney_edu_au/_layouts/15/onedrive.aspx?ga=1&id=%2Fpersonal%2Fmehala%5Fbalamurali%5Fsydney%5Fedu%5Fau%2FDocuments%2FPublications%202023%2FAJCAI2023%2FSimMining%2D3D)

Link to video: 


## Citation
If you use this dataset in your research, please consider citing:

Balamurali, M. and Mihankhah, (2023). SimMining-3D Dataset. University of Sydney. [Link to the dataset]([https://unisyd-my.sharepoint.com/:f:/g/personal/mehala_balamurali_sydney_edu_au/EuHRMzbkDShGpYv6gV3dgcIB7ZXZKb_0EvUMPU7orcbojw?e=Fox0FY](https://unisyd-my.sharepoint.com/:f:/g/personal/mehala_balamurali_sydney_edu_au/Enns61uDsTxKjCiiPM4hx9MBizoIc_T4PoeI054PmTPzzA?e=FLo13r))

Balamurali, M. and Hill, A. J. and Martinez, J. and Khushaba, R. and Liu, L.and Kamyabpour, N. and Mihankhah, E. A Framework to Address the Challenges of Surface Mining through Appropriate Sensing and Perception, 17th International Conference on Control, Automation, Robotics and Vision (ICARCV),2022, 261-267, 10.1109/ICARCV57592.2022.10004309

