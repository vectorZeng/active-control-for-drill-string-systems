# 一次实践课要求做钻柱振动的仿真，在Cheng Jun老师代码的基础上搭了一个Simulink
包括：

- 无控制的钻柱系统
- 状态观测器控制
- PID控制

![image](https://github.com/user-attachments/assets/8e8400f9-888e-44ec-8319-79d37b384c53)

效果还看得过去：

转盘转速控制：
![屏幕截图 2024-10-29 215608](https://github.com/user-attachments/assets/10f2d866-5a71-441b-9f70-d98ef09aebf7)

钻头速度控制：
![image](https://github.com/user-attachments/assets/b95d8bae-54d4-415b-b309-cbea44e69b72)


# Active control for drill-string systems
It's well known that stick-slip vibrations existing in drill-string systems are extremely severe during drilling and are expected to be mitigated or eliminated. Considering this practical problem, we present a possible solution by using observer-based tracking controller, which only requires the top measurements and is easy to implement. This repository provides the code of the conference paper "Observer-Based Tracking Control for Suppressing Stick-Slip Vibration of Drillstring System". We hope this can provide help to people who are working on the related fields.

Please note that, this code is limited to academic use only.

### Simulation figure 1:

<img src="figure/stick-slip vibration.jpg" alt="stick-slip motion" width = "500"/>
Fig. 1 Stick-slip motion of drill-string system subjected to control input (10000 Nm) and weight on bit (97347 N) 

### Simulation figure 2:

<img src="figure/system response.jpg" alt="system response" width = "500"/>
Fig. 2 Performance of drill-string system with observer based tracking controller

### Simulation figure 3:

<img src="figure/observer performance.jpg" alt="observer performance" width = "500"/>
Fig. 3 Performance of observer


If you find this helpful, please consider citing the paper
```
@article{Cheng2018ObserverBasedTC,
  title={Observer-Based Tracking Control for Suppressing Stick-Slip Vibration of Drillstring System},
  author={Jun Cheng and Min Wu and Luefeng Chen},
  journal={2018 37th Chinese Control Conference (CCC)},
  year={2018},
  pages={10254-10258}
}
```
