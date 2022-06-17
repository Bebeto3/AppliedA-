# checking the statistical summary of the dataset
data.describe()
# iterating the columns
for col in data.columns:
    print(col)
    # Remove column name 'Store ID'
#data.drop(['Store ID'], axis=1, inplace=True)
column=['Store ID ']
data.drop(column, inplace=True, axis=1)
data.head()
# Visualization of the featurs unsing Bar plot to see if there is any missing data
msno.bar(data, figsize = (16,5),color = "orange")
plt.show()
# plotting the heat map graph to see the correlation of the data in graphs 
plt.figure(figsize=(9,6))
sns.heatmap(data.corr(), vmin=-1, annot=True, cmap='YlGnBu_r')
# scattered plot for items availabel and store area...

x = data[['Items_Available']]
y = data[['Store_Area']]
_ = plt.figure(figsize=(12,8))  #increases the size of my plot
_ = plt.scatter(x , y)
_ = plt.xlabel('Items Available')
_ = plt.ylabel('Sales')
_ = plt.xticks(np.arange(0, 2800 , step = 200))  #gives a range for my x values
_ = plt.yticks(np.arange(0 ,2400 , step = 200))
plt.plot()
