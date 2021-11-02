# EVPowerSystemModel

This model is based on Simscape Electrical modeling of the power flow in an EV.
In this project, three modeling styles are used to describe the power flow model.
Single model/Model reference/System Composer
This model is very simple and should be able to be used for validation of requirement specifications and system configuration.

# The aim of this Demo model
In this project, three modeling styles are used to describe the power flow model.
1.Single model
2.Model reference
3.with System Composer
The aim of this project is to show the customer the comparison of these modeling styles.

In the style using System Composer, only the communication lines between the control unit and the hardware unit, that is the interface design, can be designed without depending on each Simulink model, and the greatest point is that the results can be reflected in each Simulink model.

# How to Use the Model
## 1. Single model
<img src="/uploads/5dfb4732f850da410f45ca9a3cb97c67/Snag_1e3316ff.png" width=50%>  

The top model has Knob built in the dashboard.
Please start the simulation and change the values as Knob.
The simulation parameters will be changed according to the power command value and load power consumption.

## 2. Model Reference / with System Composer
<img src="/uploads/307be6a54ebbeed1376400e15705b2fc/Snag_1e355e10.png" width=40%>
<img src="/uploads/f51271c9de42a428ea37562499796962/Snag_1e3567f4.png" width=50%>  

The dashboard is not available in Model Reference.
Therefore, load the .m file saved in the InputSignalData folder to manipulate the power command value and load power consumption.
Press the Simulation Run button to start the simulation according to the input signal defined in ImputSignal.

# Contact
Please Contact me if you have any questions about this Model.
Thank you!

Yuki Kamtani Apprication Engineer @ MatnWorks Japan
ykamatan@mathworks.com
