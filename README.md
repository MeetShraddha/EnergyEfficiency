# EnergyEfficiency

Dataset reference: https://archive.ics.uci.edu/dataset/242/energy+efficiency

This study looked into assessing the heating load and cooling load requirements of buildings (that is, energy efficiency) as a function of building parameters.

Summary: We perform energy analysis using 12 different building shapes simulated in Ecotect. The buildings differ with respect to the glazing area, the glazing area distribution, and the orientation, amongst other parameters. We simulate various settings as functions of the afore-mentioned characteristics to obtain 768 building shapes. The dataset comprises 768 samples and 8 features, aiming to predict two real valued responses. It can also be used as a multi-class classification problem if the response is rounded to the nearest integer.

Variable_info: The dataset contains eight attributes (or features, denoted by X1...X8) and two responses (or outcomes, denoted by 'target_col': ['Y1', 'Y2'])

name     role        type demographic                description units  
0   X1  Feature  Continuous        None       Relative Compactness  None   
1   X2  Feature  Continuous        None               Surface Area  None   
2   X3  Feature  Continuous        None                  Wall Area  None   
3   X4  Feature  Continuous        None                  Roof Area  None   
4   X5  Feature  Continuous        None             Overall Height  None   
5   X6  Feature     Integer        None                Orientation  None   
6   X7  Feature  Continuous        None               Glazing Area  None   
7   X8  Feature     Integer        None  Glazing Area Distribution  None   
8   Y1   Target  Continuous        None               Heating Load  None   
9   Y2   Target  Continuous        None               Cooling Load  None


<img width="936" height="790" alt="image" src="https://github.com/user-attachments/assets/9fb4b4fe-741c-49d3-b824-b2bf0e25fc22" />



<img width="2485" height="2490" alt="image" src="https://github.com/user-attachments/assets/77a7fe32-7792-4ebe-8780-8c0e02b48e69" />


                      Model    MSE  R2_Y1 (Heating Load)  R2_Y2 (Cooling Load)
0         Linear Regression   9.52                  0.91                  0.89
1             Random Forest   1.94                  1.00                  0.96
2         Gradient Boosting   1.28                  1.00                  0.98
3  Support Vector Regressor  30.31                  0.69                  0.69
4                   XGBoost   0.45                  1.00                  0.99
