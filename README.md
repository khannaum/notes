# notes
Create  Notes
#Pandas percentage of total with groupby
#solution one 
P=HXC.groupby('Nav HXC Node')[u'Ussd Total',u'Ussd Success'].sum().reset_index()
P['Percentage'] = 100 * P['Ussd Success']  / P['Ussd Total'].sum()

