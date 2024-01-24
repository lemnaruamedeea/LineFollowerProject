# 🚘 Line Follower Project - Robotics Hackathon 🚘

This final project developed during the Introduction To Robotics course consists of building, assembling and programming a robot whose objective is to follow a black line on a track and complete it as fast as possible. In order to do so, me and my colleagues spent 12 hours at the university, where we developed our robots in teams of three. 🙊🙈🙉

My team - Powerpuff Girls: 💙❤️💚
@vfranci
@Diana5B

<details>
<summary><h2>Project and Design Description 📏📝</h2></summary>

### Project components: 🛠️
- Arduino Uno
- Power source: LiPo battery
- Two wheels
- QTR-8A reflectance sensor
- Ball caster
- L293D motor driver
- Two DC motors
- Medium breadboard
- Wires (M - F, F - F), zip-ties, screws as needed

For the chassis we cut into a foam board after measuring an apropriate distance between the wheels and for the sensor. We secured the breadboard,the Arduino board and the motors using zip-ties. 

### Requirements ⏲️

Minimum requirements for the project were to have the robot finish the line follower track, including the curved lines. To achieve maximum grade, the course had to be finished in under 20 seconds and, upon starting, the sensor had to be calibrated using automatic motor movement. 🏎

### Software implementation 💻

The robot calibrated its sensor by moving left and right in order to recognize the black line it had to follow. The movement behaviour was determined by using a proportional-integrative-derivative controller. We started with a simple code provided by our teacher in which we had to alter the kp, ki, and kd values to achieve the desired movement. We started by assigning random values to the proportional constant in order to observe the behaviour. Once the robot was able to take the turns without overshooting, we began updating the kd value to smooth the wobble. 

The final values were:
kp = 4.3;
ki = 0.000;
kd = 23.2;

Afterwards, we implemented the automatic calibration and juggled the tresholds for the error and motor speed values.

</details>

<details>
<summary><h2>Performance and outcome 🏁🏎️</h2></summary>

Final setup of the car: 
![Car](https://github.com/lemnaruamedeea/LineFollowerProject/blob/main/LineFollower/Car.jpg?raw=true)

  <img src="https://github.com/lemnaruamedeea/LineFollowerProject/blob/main/LineFollower/Car.jpg?raw=true" alt="Empty" width="1000" />

When presenting our design, the lowest time recorded for completing the track was 17.871 seconds. 🎉🎊

Performance video on [YouTube](https://youtube.com/shorts/aUqb2nQzOtc?si=vIdgjRWChrSpdg4H).

</details>
