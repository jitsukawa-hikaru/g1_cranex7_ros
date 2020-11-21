<<<<<<< HEAD

# G1_cranex7_ROS  
=======
# g1_cranex7_ros
>>>>>>> origin

設計製作論3　1班の最終発表用のCRANE-x7のROSパッケージです。  
  
  
  


#  動作環境 
  
以下の環境で動作確認を行っています。  
・ROS Melodic  
　・OS: Ubuntu 18.04.5 LTS  
　・ROS Distribution: Melodic Morenia 1.14.3  
　・Rviz 1.13.13  
　・Gazebo 9.0.0  
   
 ---
 
 
  
###  gazebo上でシミュレーションを行う場合
  
シミュレータを使う場合、以下のコードを実行します。  

```sh
<<<<<<< HEAD
roslaunch G1_cranex7_ROS crane_x7_with_table.launch
=======
roslaunch g1_cranex7_ros crane_x7_with_table.launch
>>>>>>> origin
```  
---

###  実機を使う場合  
  
 
 制御信号ケーブルを接続した状態で次のコマンドを実行します。  
 ```sh
 sudo chmod 777 /dev/ttyUSB0  
 roslaunch crane_x7_control crane_x7_control.lanch  
 ```

---

   
## 実行方法  
  
・bottle_pick.py  
中間発表で発表したCRANE_X7にボトルを振らせるコードです。  
ボトルを設置した後、crane_x7_examples下にあるbottle_pick.pyを実行します。  
  

```sh
<<<<<<< HEAD
rosrun G1_cranex7_ROS bottle_pick.py 
=======
rosrun g1_cranex7_ros bottle_pick.py 
>>>>>>> origin
```  
    
ボトルは以下のように設置してください。  
<img src=https://github.com/robotcreating2020-1/images/blob/master/2020-11-15_1.png width=500px />  
  
アームがボトルをつかんだ後、ボトルを6回ほど振り、机に置きます。  
  
ボトルを振るジョイントはfor文の中で直接指定しているので、容易に変更可能です。(デフォルトでは0番と6番を指定)  
また、動かす角度も変えられます。(デフォルトでは0番を30度、6番を55度にしています。)  
  
---
  
### gazebo上での動作  
  
gazebo上での動作は以下のようになります。  
<img src=https://github.com/robotcreating2020-1/images/blob/master/Sim_SoE.gif width=500px />  
  
---
  
### 実機での動作  
  
実機での動作は以下のようになります。  
<img src=https://github.com/robotcreating2020-1/images/blob/master/State_of_Execution.gif width=500px /> 

---
  
