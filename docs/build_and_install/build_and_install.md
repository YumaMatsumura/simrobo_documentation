# ビルド&インストール手順
## インストール手順
以下のコマンドで関連パッケージのインストールを行う。  
```bash
sudo apt install ros-foxy-joint-state-publisher ros-foxy-joint-state-publisher-gui ros-foxy-xacro ros-foxy-ros2-control ros-foxy-ros2-controllers ros-foxy-gazebo-ros2-control ros-foxy-joy-linux
```

次に、ROS2のワークスペースを作成し、本パッケージをインストールする。  
```bash
mkdir -p ~/ros2_ws/src && cd ~/ros2_ws/src
```

```bash
git clone https://github.com/YumaMatsumura/simrobo.git
```

## ビルド手順
ワークスペースに戻り、ビルドする。
```bash
cd ~/ros2_ws
```

```bash
colcon build --symlink-install
```
