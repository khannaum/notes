# notes
Create  Notes
#Pandas percentage of total with groupby
#solution one 
P=HXC.groupby('Nav HXC Node')[u'Ussd Total',u'Ussd Success'].sum().reset_index()
P['Percentage'] = 100 * P['Ussd Success']  / P['Ussd Total'].sum()

Nav HXC Node  Ussd Total  Ussd Success  Percentage
0    hxcslc-a01           0             0    0.000000
1    hxcslc-a02           0             0    0.000000
2    hxcslc-a03           0             0    0.000000
3    hxcslc-a04           0             0    0.000000
4    hxcslc-a05           0             0    0.000000
5    hxcslc-a06           0             0    0.000000
6    hxcslc-a07           0             0    0.000000
7    hxcslc-a08           0             0    0.000000
8    hxcslc-a09           0             0    0.000000
9    hxcslc-a10           0             0    0.000000
10   hxcslc-a11           0             0    0.000000
11   hxcslc-a12           0             0    0.000000
12   hxcsvc-a01       33605         31792   11.821136
13   hxcsvc-a02       33648         31932   11.873192
14   hxcsvc-a03       33597         31771   11.813328
15   hxcsvc-a04       33616         31739   11.801429
16   hxcsvc-a05       33598         31761   11.809610
17   hxcsvc-a06       33621         31818   11.830804
18   hxcsvc-a07       33621         31855   11.844561
19   hxcsvc-a08       33636         31780   11.816674
