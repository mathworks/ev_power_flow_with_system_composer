# Copyright
Copyright 2021 - 2022 The MathWorks, Inc.

# EVPowerSystemModel
This model is based on Simscape Electrical modeling of the power flow in an EV.
In this project, three modeling styles are used to describe the power flow model.
Single model/Model reference/System Composer
This model is very simple and should be able to be used for validation of requirement specifications and system configuration.

このモデルは、Simscape ElectricalによるEV内のパワーフローのモデリングです。
このプロジェクトでは、パワーフローモデルを記述するために3つのモデリングスタイルを使用しています。
単一モデル/モデルリファレンス/System Composer
このモデルは非常にシンプルで、要求仕様やシステム構成の検証に使用できるはずです。

# The aim of this Demo model
In this project, three modeling styles are used to describe the power flow model.
1.Single model
2.Model reference
3.with System Composer
This project will make it possible to compare these modeling styles.

In the style using System Composer, only the communication lines between the control unit and the hardware unit, that is the interface design, can be designed without depending on each Simulink model, and the greatest point is that the results can be reflected in each Simulink model.

このプロジェクトでは、パワーフローモデルを記述するために3つのモデリングスタイルを使用しています。  
1.シングルモデル  
2.モデル参照  
3.System Composerを使用  
このプロジェクトによってこれらのモデリング・スタイルの比較が可能になります。

System Composerを用いたスタイルでは、各Simulinkモデルに依存することなく、制御ユニットとハードウェアユニット間の通信線、つまりインターフェース設計のみを設計することができ、その結果を各Simulinkモデルに反映させることができるのが最大のポイントです。

# How to Use the Model
## 1. Single model
<img src="/uploads/5dfb4732f850da410f45ca9a3cb97c67/Snag_1e3316ff.png" width=50%>  

The top model has Knob built in the dashboard.
Please start the simulation and change the values as Knob.
The simulation parameters will be changed according to the power command value and load power consumption.

トップモデルには、ダッシュボードにKnobが組み込まれています。
シミュレーションを開始して、Knobとしての値を変更してください。
シミュレーションのパラメータは、電力指令値や負荷の消費電力に応じて変更されます。

## 2. Model Reference / with System Composer
<img src="/uploads/307be6a54ebbeed1376400e15705b2fc/Snag_1e355e10.png" width=40%>
<img src="/uploads/f51271c9de42a428ea37562499796962/Snag_1e3567f4.png" width=50%>  

The dashboard is not available in Model Reference.
Therefore, load the .m file saved in the InputSignalData folder to manipulate the power command value and load power consumption.
Press the Simulation Run button to start the simulation according to the input signal defined in ImputSignal.

ダッシュボードは、モデルリファレンスでは利用できません。
そのため、InputSignalDataフォルダに保存されている.mファイルをロードして、電力指令値や負荷の消費電力を操作します。
Simulation Runボタンを押すと、ImputSignalで定義した入力信号に応じてシミュレーションが開始されます。

# Required Toolboxes
MATLAB&reg;/
Simulink&reg;/
System Composer&trade;/
Simscape&trade;/
Simscape Electrical&trade;/
DSP System Toolboxes&trade;

# Recomend Toolbox
Control System Toolbox&trade; 

モデルの伝達関数を表示するのに必要です。
SycnADC_WithFBParam.mの13行目以降をコメントアウトすればこのToolboxがなくてもモデルは動作します。

It is needed to display the transfer function of the model.
If you comment out line 13 onwards of SycnADC_WithFBParam.m The model will work without this Toolbox.
