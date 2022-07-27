# Gazebo環境でジョイコン操作
## empty_worldでのジョイコン操作
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

## ロボットのスポーン位置を変更する
Gazebo上のロボットスポーン位置はsimrobo\_gazebo/launch/empty\_world.launch.pyのspawn_entityを編集する。  
```python
spawn_entity = Node(
    package='gazebo_ros', 
    executable='spawn_entity.py',
    arguments=['-entity', 'simrobo',
                    '-x', '0.0',
                    '-y', '0.0',
                    '-z', '0.2',
                '-topic', '/robot_description'],
    output='screen'
)
```
