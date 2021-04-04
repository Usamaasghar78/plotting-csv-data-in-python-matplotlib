in this csv file here is the data of two companys displayed in three colums as company name,model and price.
lets jump to the code

first i imported matplotlib.pyplot as plt
then i imported pandas as pd

then i wrote "plt.style.use('bmh')" just for the design of the graph but its not necessiarily needed.
then i created a data read variable that reads csv file "df = pd.read_csv('prices.csv')"

in all brands section 'x' reads the models and 'y' reads the prices of all brands

in specified brands section 'x' and 'y' works in the same way as of all brands section but the difference is we can specify which brands data is to be plotted.

in bar chart section 
"plt.xlabel('Model', fontsize=18)"
 "plt.ylabel('Price($)', fontsize=16)"
 the above lines are used to label the x and y axis and "plt.bar(x, y)" plots the graph
 
in pie chart section
"plt.pie(y, labels=x, radius=1.2,autopct='%0.01f%%', shadow=True, explode=[.05,.2,.05,.2,.05,.2,.05])"
plt.pie method y and labels=x are necessary and other variables are just for the better represenation of the graph

in line graph section
" plt.xlabel('Model', fontsize=18)" used to label x axis
" plt.ylabel('Price($)', fontsize=16)" used to label y axis
 "plt.scatter(x, y)" used to get a scattered graph
 "plt.plot(x, y)"  used to get the line graph
 but we can run both the commands together to get a more appealing graph
 
" plt.show()" used to show the plotted graph
