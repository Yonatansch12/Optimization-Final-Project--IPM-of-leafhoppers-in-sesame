# -Optimization-Final-Project--IPM-of-leafhoppers-in-sesame
This project model the optimization of pesticide the leafhopper in sesame crops. 

## Introduction
The subject of this project is the integrated pest management (IPM) of the leafhopper (Orosius orientalis). who causes significant damage to sesame crops through its sap-sucking habits and its role as a vector for Phyllody disease. By eating the plant sap, both nymphs and adults induce curling of leaf edges, leaf discoloration, and premature leaf shedding, which weaken the plants and reduce their photosynthetic capability. More critically phyllody disease transforms floral parts into green leaf-like structures which cause severe yield losses ranging from 34% to 100%. Effective management of this pest is essential to protect sesame crop health and productivity.

Therefore, we propose a model to optimize the control of the leafhopper population on sesame crops while minimizing economic costs.

## Model
Variables and parameters:<br />
- Population dynamics of leafhopper: birth and pesticide effect.<br />
- Sesame crop characteristics: market value, yield, damage taken.<br />
- Pesticide efficiency - chemical, biological, and IPM (combined) <br />
- Economic factors: costs of damage, pesticides, and applications.<br />
 
## Objective function:
Minimize the total cost of pest management, including the costs of pesticide prices, applications, and economic losses due to leafhoppers. Financial losses are calculated based on the reduction in seeds by 10 leafhoppers per plant, infestation,  and the average value of the sesame crop for oil.

minimize Total Cost= t=0weeks-1(damages (t)+treatment costs(t))


## Constraints: 
- leafhopper population dynamics: considering only birth, carrying capacity of 10,000, and the impact of pesticide applications. <br />
- Constant market value and costs: The market value of sesame and the pesticide costs remain the same throughout the season.<br />
- Pesticide application limits: only once a week.<br />
-Homogeneity: Regarding soil quality, climate conditions, leafhopper distribution, and pesticide application are all homogeneous in the field.<br />
- Pesticide resistance = none. <br />

## Variables definitions
r= Reproduction rate= 4 times per week<br />
K = Carrying capasity= 10,000<br />
Ec= chemical pesticide efficiency= 0.85%<br />
Eb= biological pesticide efficiency =0.7%  <br />
Ecomb=IPM efficeicy=0.95% <br />
k= Yield loss= 1.5 planet per 10 leafhopers<br />
Cc= Chemical pesticide cost= 6 $ per treatment<br />
Cb=Biological pestiside's cost= 7.35 $ per treatment <br />
Ccomb=IPM pestiside's cost= 6.675 $ per treatment <br />
P=  Sesame's Market price= 2.4 $ per kg<br />
Cd= 0.048 $ per damaged plant<br />
Cp= Cost of pesticise application = 10 $  per hour<br />

## Equations and developing Variables :

Population dynamics:<br />
r= reproductive rate=4 times each week <br />
K=carrying capacity =10,000<br />
Ec= chemical pesticide efficiency= 0.85%<br />
Eb= biological pesticide efficiency =0.7%  <br />
Ecomb=IPM efficeicy=0.95% <br />

pop (t)=population(t-1)+rpopulation(t-1)(1-population(t-1)K)-Ei(population(t-1) 


Sesame’s market value:
As observed in the first weeks of the sesame season, in the plots of Professor Tzvika Peleg's research laboratory, we have estimated that each plot suffers a total loss of 1.5 plants. this disease requires the removal of these plants. Additionally, after counting dozens of samples, we found that, on average, there are 60 pods per plant, each containing about 70 seeds. This means that one plant represents an average loss of 6,300 seeds. Converting this to weight results in a loss of 20 grams of dry matter (ready seeds) per plant. There are 450 plots in the field, resulting in an estimated total loss of 9 tons of seeds. Given the average market price of sesame seeds (2.4 dollars per kg), the estimated loss amounts to 21,600 dollars for the first week and 0.048 dollars per damaged plant. 


Pesticide application and costs:

Chemical- Based on professional experience, observations, and different resources, we found that the average concentration for using chemical pesticides is 2.5 ml when 30 ml of the substance is required for 12 liters of water (the volume of the sprayer). The pesticide market price stands at 34$ per liter. One sprayer takes about 30 minutes to operate, with the labor cost being $10 per hour. Consequently, we calculated that a single treatment costs $6.

Biological- Based on the same assumptions as above, we found that a single biological treatment requires an average of 300 grams of material. The pesticide cost is $22 per kilogram, resulting in a single treatment cost of $7.25.

Combined- Assuming that an integrated pest management treatment is evenly divided between the types of treatments, the cost of a single such treatment would be $6.675.

based on articles, research, and assumptions we found that 10 leafhoppers cause irreversible damage to 1.5 plants.  
