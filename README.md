# Hotel-Bookings
EDA for the Hotel Booking
Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests? This hotel booking dataset can help you explore those questions!
This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things. All personally identifying information has been removed from the data.
Explore and analyze the data to discover important factors that govern the bookings.

he most difficult thing in life is to know yourself'

This quote belongs to Thales of Miletus. Thales was a Greek/Phonecian philosopher, mathematician and astronomer, which is recognised as the first individual in Western civilisation known to have entertained and engaged in scientific thought (source: https://en.wikipedia.org/wiki/Thales)

I wouldn't say that knowing your data is the most difficult thing in data science, but it is time-consuming. Therefore, it's easy to overlook this initial step and jump too soon into the water.

So I tried to learn how to swim before jumping into the water. Based on Hair et al. (2013), chapter 'Examining your data', I did my best to follow a comprehensive, but not exhaustive, analysis of the data. I'm far from reporting a rigorous study in this kernel, but I hope that it can be useful for the community, so I'm sharing how I applied some of those data analysis principles to this problem.

Despite the strange names I gave to the chapters, what we are doing in this kernel is something like:

Understand the problem. We'll look at each variable and do a philosophical analysis about their meaning and importance for this problem.
Univariable study. We'll just focus on the dependent variable ('SalePrice') and try to know a little bit more about it.
Multivariate study. We'll try to understand how the dependent variable and independent variables relate.
Basic cleaning. We'll clean the dataset and handle the missing data, outliers and categorical variables.
Test assumptions. We'll check if our data meets the assumptions required by most multivariate techniques.
 So... What can we expect?
In order to understand our data, we can look at each variable and try to understand their meaning and relevance to this problem. I know this is time-consuming, but it will give us the flavour of our dataset.

In order to have some discipline in our analysis, we can create an Excel spreadsheet with the following columns:

# Variable - Variable name.
Type - Identification of the variables' type. There are two possible values for this field: 'numerical' or 'categorical'. By 'numerical' we mean variables for which the values are numbers, and by 'categorical' we mean variables for which the values are categories.
#Segment - Identification of the variables' segment. We can define three possible segments: building, space or location. When we say 'building', we mean a variable that relates to the physical characteristics of the building (e.g. 'OverallQual'). When we say 'space', we mean a variable that reports space properties of the house (e.g. 'TotalBsmtSF'). Finally, when we say a 'location', we mean a variable that gives information about the place where the house is located (e.g. 'Neighborhood').
# Expectation - Our expectation about the variable influence in 'SalePrice'. We can use a categorical scale with 'High', 'Medium' and 'Low' as possible values.
#Conclusion - Our conclusions about the importance of the variable, after we give a quick look at the data. We can keep with the same categorical scale as in 'Expectation'.
#Comments - Any general comments that occured to us.

# We encountered following patterns in the given historical data:
1.Top Hotel - City Hotel. Top Agent - Agent No. 9. Top room type - A
2.One out of every three bookings are cancelled.
3.People prefer to tour more in August.
4.Most preferred meal is BB (Bread and Breakfast.
5.Online marketing is the best way to attract customers.
6.People do not want to pre-deposit the money for booking.
7.Only 10% of people require parking space.
8.Most of the visitors are couples.
9.The Resort hotel is preferred mostly for longer stays, day time stays. and when the parking space is needed.
10.More than 15 days advance bookings have high chances of cancellation.
11.Assigning a different room is not a reason for cancellation.
12.Direct bookings have very less cancellation%.
13.Best time to book a hotel is in January.
14.Average days in advance booking: 77 days
15.Average nights spent by visitors: 3.
16.Most visitors are from Portugal, Britain, France, Spain and Germany.
17.Total Special requests and the revenue depends more on total members arrived.

# Inferences and Conclusion
Conclusion
That's it! We reached the end of our exercise.

Throughout this kernel we put in practice many of the strategies proposed by Hair et al. (2013). We philosophied about the variables, we analysed 'SalePrice' alone and with the most correlated variables, we dealt with missing data and outliers, we tested some of the fundamental statistical assumptions and we even transformed categorial variables into dummy variables. That's a lot of work that Python helped us make easier.

But the quest is not over. Remember that our story stopped in the Facebook research. Now it's time to give a call to 'SalePrice' and invite her to dinner. Try to predict her behaviour. Do you think she's a girl that enjoys regularized linear regression approaches? Or do you think she prefers ensemble methods? Or maybe something else?

It's up to you to find out.
