# Gazebo環境でジョイコン操作
まず、以下のコマンドでGazeboとRViz2を起動する。  
```bash
ros2 launch simrobo_gazebo empty_world.launch.py
```

![Bringup RViz Image](https://github.com/YumaMatsumura/simrobo_documentation/blob/master/images/tutorial/bringup_rviz.png)
![Bringup Gazebo Image](https://github.com/YumaMatsumura/simrobo_documentation/blob/master/images/tutorial/bringup_gazebo.png)

起動したら、ドライバーを起動し、ジョイコン操作できる状態にする。  
```bash
ros2 launch simrobo_driver driver.launch.py
```

ジョイコン操作することで、Gazebo上のロボットモデルが動作する。  
