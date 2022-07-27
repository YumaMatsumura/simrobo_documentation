# Simroboについて

simroboパッケージのgithub-url： [simrobo github url](https://github.com/YumaMatsumura/simrobo)

## Simroboパッケージとは
差動二輪ロボットを簡単にROS2でシミュレートしたいときに使用できるものである。  
simrobotは、STLファイルを使用せず、直方体、球、円柱などの単純な立体で構成されたロボットであり、読み込み速度を向上させている。

## Simroboパッケージの構成
* simrobo\_description：simroboのロボットモデルを含んでいるパッケージである。
* simrobo\_driver：simroboのオドメトリやtfなどを計算しているパッケージである。
* simrobo\_gazebo：Gazebo起動のLaunchファイルを含んでいるパッケージである。
