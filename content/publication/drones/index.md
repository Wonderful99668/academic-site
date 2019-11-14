---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Image-based Visual Servoing with Quadrotor in a Newer Experimental Platform"
subtitle: "Key words: PX4; OpenCV; ROS; Vicon"
authors: 
- admin

# Schedule page publish date (NOT publication's date).
publishDate: 2019-08-26

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
# publication_types: ""

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: In recent years rotary-wing unmanned aerial vehicles (UAVs) are seeing more uses in applications such as transmission line inspection, event filming, parcel delivery, and search-and-rescue missions.

# Summary. An optional shortened abstract.
summary: ""

tags: ["Robotic", "Drones"]
categories: []
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

# url_pdf:
# url_code:
# url_dataset:
url_poster: drone.pdf
# url_project:
# url_slides:
# url_source:
url_video: https://www.youtube.com/watch?v=Nkaf59vUjKM

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Drone"
  focal_point: Smart
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

In recent years rotary-wing unmanned aerial vehicles (UAVs) are seeing more uses in applications such as transmission line inspection, event filming, parcel delivery, and search-and-rescue missions. Recent improvements in embedded systems have lead to more research for improving unmanned aerial vehicle (UAV) autonomy. Traditionally for outdoor use, the inertial measurement unit (IMU) with magnetometer, barometer, or global positioning system (GPS) can be used for pose estimation, where the pose estimate is used for motion control. However, in GPS denied environments, such as indoors, other sensors need to be used for acquiring pose of the UAV in the environment. One method to solve for the vehicle’s pose is visual servoing, which uses a camera to collect information about the environment, and estimates the UAV’s pose for control. This posts implements a newer experimental platform to improve the quatrotor visual servoing performance. This new platform utilizes the Robot Operating System (ROS) running on an on-board Nvidia Jetson TX1 (TX1) mini computer with a FLIR Chameleon 3 camera for the computer vision (CV) system. ROS is chosen to create a simple framework that would handle necessary components for the UAV, such as image capture and data transfer, while allowing for minimal software changes to test different algorithms. Using this framework, future research projects using the platform can save time troubleshooting issues testing hardware, and instead focus on problems related to the algorithms being tested. Also, future upgrades to the platform would need minimal changes to the software so long as the new system is able to run ROS. For the experiments, the CV system uses color to identify visual features used to compute image moments which are sent to a PX4 flight management unit (FMU) for control of the UAV over a target.