# CMOS-inverter-2
***This is the part 2 of the CMOS-inverter. I've discussed the further concepts related to the inverter like noise margin,propagation delay,rise and fall time etc.***
***
In the previous repo CMOS-inverter i had discussed the basic concepts of the inverter.This will be a continuation to the previous discussion. Lets explore more about our inverter and see what it has got more to provide to us. I'll be frequently updating the repository.<br />
<br />
**Note:
      Length:180nm
      PMOS Width Wp: 800nm
      NMOS Width Wn: 400nm**
***
### Contents
***
***
***
***
***
***
## 1.Transient Analysis
## 1.1 Review
Lets quickly look into the behaviour of the inverter.The input to the the inverter is a square wave with **Rise time and Fall time of 2ns**,**T(on)=10ns** and the period of the input wave is **T(period)=20ns**.As you can see the signal gets inverted and output.<br />
<br />
**Schematic:**
![CMOS inverter-2](./images/tran1sch.png)<br>
**Output:**
![CMOS inverter-2](./images/tran1.png)<br>
## 1.2 Variation in load Capacitence (cload).
Lets try plotting the output voltage of an inverter for different values of load capcitance.There's certain amount of delay introduced as the capacitence value increases.Certainly this is not desired,closely observed for higher values the output wpnt reach to full VDD.So we will have to always keep in mind the maximum and minimum load capacitence while designing
![CMOS inverter-2](./images/tanscap.png)<br>
![CMOS inverter-2](./images/trancapop.png)<br>
Now lets analyise the output signal.Closely observe the propagation delay in the output.
***
## 1.3 Rise-Time and Fall-Time
![CMOS inverter-2](./images/theoimages/th1.png)<br>
### Fall-Time
Fall time is defined as the time taken for the output signal from 90% of final value to 10% of the final value.The difference between these time interval yields the fall time (**tfall**).<br />
![image](https://user-images.githubusercontent.com/67727794/222906879-193febbf-f2c5-4681-9b7f-4a5838ab063c.png)
![image](https://user-images.githubusercontent.com/67727794/222906952-6b290238-2ca7-4bae-afda-cc06d13f5824.png)
<br />
### Rise Time
Rise time is defined as the time taken for the output signal from 10% of final value to 90% of the final value.The difference between these time interval yields the rise  time (**trise**).<br />
![image](https://user-images.githubusercontent.com/67727794/222907650-6e0c49ea-a06a-4ede-a62c-c2bb95820d5d.png)
![image](https://user-images.githubusercontent.com/67727794/222907521-6abf32d8-4688-4da2-94fe-dfe95b452dde.png)
<br />
That was bit of theory to get started with our analysis.I always want a crisp theoritical understanding anf then move into the simulation.The Below figure shows the simulation out for the rise time and fall time.
