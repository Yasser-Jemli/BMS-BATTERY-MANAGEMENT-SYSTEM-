# BMS-BATTERY-MANAGEMENT-SYSTEM-


BMS ( battery management system ) 

INTRODUCTION  : 

The storage battery control system (Battery Management System or BMS in English, or Battery State of Charge Box or BECB in French) is an electronic system allowing the control and charging of the various elements of a storage battery. .

Battery protection
A BMS protects its battery by preventing it from operating outside of its typical operating range:
overcurrent.
power surge (when charging).
undervoltage (during discharge), especially important for lead-acid and Li-ion cells.
overheated.
under temperature.
over-pressure (NiMH batteries)

The BMS prevents the battery from operating outside of its typical operating range, through:
an internal switch.
devices external to the battery that allow its use to be reduced or terminated.
environmental control, such as heaters, fans, air conditioners or liquid coolants.




Select Voltage , Current and batteries :

Ok, first of all you need to have in mind what kind of battery pack you want to make. For that I check the specs of my system. I will use the Samsung INR18650 LiIon batteries . The nominal voltage of these batteries is 3.7V. 

Series or parallel :
Ok so I want the maximum voltage for my ESCs and motors that is 26V. Each of these batteries have a nominal voltage of 3.7V and a maximum voltage when fully charged of 4.2. For more check the datasheet of the batteries So, if I want around 12V, with 4.2V batteries I need 3 batteries in series and get a total maximum voltage of 25.2V. We know that batteries in series will sum their voltages but have the same capacity and in parallel they sum the capacity but have the same voltage. 
























































































Ok, now we know we need 3 batteries in series. But what about capacity. Each of these 7INR18650 have a capacity of 3000mAh. That means it could deliver 3A for an hour or 1A for 3 full hours. But that value is not always perfect. I want more capacity so, in addition to having 6 batteries in series, each of these batteries will actually be a pack of 2 batteries in parallel. So I will have 3 packs in series of 2 x 4.2V batteries in parallel and that will give me a total of 12.6V and a capacity of 6000mAh. 

we need t o make sure that all the batteries should be the some or we can have a problem could lead to a fire 



Schematic:

 


To charge the batteries, the manual recommends a CC and CV or better said constant current and constant voltage. So, if I put my power supply to 12.6V and 3A the batteries will get charged. But that will damage the batteries over time since one battery could get charged faster than others. For that we need a balanced charging process. We need a battery management system or BMS. Use the schematic below to connect the BMS to the batteries. 


OUR BMS : 
















 Suitable for lithium batteries with nominal voltage 3.7V and full voltage 4.2V (including 18650,26650, polymer lithium battery) without external size limit. Suitable for starting electric drills.
Charging voltage: 12.6V - 13.6V.


Continuous discharge current (upper limit):


 40A (if the cooling environment is not good, please reduce the charging current).


Continuous charging current (upper limit): 20 A
