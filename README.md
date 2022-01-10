The assignment mimics the basic operation of a Jewellery Store. 

It contains:
• Backend in .Net/ASP.NET Core and Database can be local DB / In memory

**Requirement:**
We require that the candidate should implement atleast two functionalities to handle the Jewellery Store operations.
The description of the expected functionalities are as follows:
a) Login - It allows only the pre-registered users to login. It takes two mandatory parameters which are of string type - (i) Username (ii) Password
b) Calculate total price - This method (or endpoint) will be protected. Until and unless the user has not logged-in, he/she should not be able to access this method (or endpoint).
Upon trying to access it without logging-in, a 404 status code or a message stating "Unauthorized User" should be returned.
It takes following parameters:
(i) Gold price (per gram) - This is a required parameter and accepts only numerical value, which contains the price of gold per gram.
(ii) Weight of the item (in grams) - This is a required parameter and accepts only numerical value, which contains the weight of the gold in grams.
(iii) Discount (in percentage) - This is an optional parameter and accepts only numerical value. It contains the discount percentage.

The method (or API endpoint in case of RESTful implementation) returns the total price based on the formula: (Gold price per gram * weight) - discount
For Example:
(1) Gold price = 1000
Weight of the item (in grams) = 10
Discount (in percentage) = NULL

Thus, total price of the item => (1000 * 10) = 10000

(2) Gold price = 1000
Weight of the item (in grams) = 10
Discount (in percentage) = 5

Thus, total price of the item => (1000 * 10) - Discount = 10000 - (5% of 10000) = 9500

**Note**:
No need for any registration of user. By default, you can store the users either in local DB/in memory.

**Expectations**:
The candidate is at free-will to implement the given assignment either as a console application or as a RESTful API application.
Please use best practices everywhere.
In case of RESTful API application, swagger documentation is not mandatory, but if provided, it would be helpful.
