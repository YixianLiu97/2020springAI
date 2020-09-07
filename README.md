# Flatten Indianapolis

The goal for this robot is to flatten the Indianapolis. 


## Author

- Yixian Liu


## Homework 3 Questions

- whatever illustrations or figures you create. Also include a 1-3 pages of text 
  (you should refer to your illustrations) explaining.
  
  - myRobot state chart
   ![myRobot](https://github.com/YixianLiu97/2020springAI/blob/master/myRobot.png)
   
     - the state chart has two part, the environment and the agent. The sensor gets the 
     
  
   
  - myRobot appearance
   ![myRobotPic](https://github.com/YixianLiu97/2020springAI/blob/master/myRobotPic.jpeg)
   
     - the appearance of my robot is like a airship.
        
    
- how your robot works.

    - When the robot starts and flies in the low-level sky of Indianapolis. it will check 
    the city with the GPS and its cameras that is the city in the fire. If the city is not 
    in the fire, my robot will start to destroy Indianapolis with fuel and fire.First, it 
    will scan the area and see how big it is. If the area is small, then it will ignite the 
    area with fire directly. If the area is over five acres of land, then it will sprinkle 
    the area with fuel and ignite the area. It will go over then the whole map once first, 
    and then check the city with cameras to make sure the whole city is in the fire. If some 
    part of the city is not in the fire, then it will go to the area and do the destroy part 
    again.

- the P, E, A, S parts of your robot.

    - Performance Measure: fast, no traffic, fire the city completely.
    
    - Environment: in the low level(altitude) of the city sky
    
    - Actuators: sprinkle gas with oil gun, sting-out with fire gun
    
    - Sensors: cameras, GPS.



- the environment type in terms of the seven properties found in section 2.3.2 of R&N 
  (e.g., fully observable vs. partially observable, single agent vs. multiagent etc.). 
  For any property that is not obvious, please explain.
  
   - Observable: **Full Observable**
   
   - Agents: **Single**
   
   - Deterministic: **Deterministic**
   
        my robot is in fully observable environment, so it's also in deterministic 
        environment.
   
   - Episodic: **Sequential**
   
        my robot is in sequential environment because the first decision will influence 
        the all future decisions and actions. For example, if the robot check the map and
        decide fire this area without the fuel, and later the area is not in fire totally,
        then it should come back and fire the are again.
   
   - Static: **Dynamic**
   
        my robot need check the map if the whole city in the fire or not. If somewhere still
        not in fire, it should go to the area and fire it.
   
   - Discrete: **Discrete**
   
        my robot is a discrete-state agent: the way it sprinkle gas and fire is discrete-time,
        it need fly to the area, check the area and then decide if it needs sprinkle gas or 
        fire the area directly.
   
   - Know: **Unknown**
   
        there is no rule like "law of physics" for my robot to follow the decision. It should
        learn and make decision by itself, so it's Unknown environment.
  
  
  
- what type of agent (simple reflex, model-based, goal-based, or utility-based) is it? 

   - My robot is **goal-based** agent. 