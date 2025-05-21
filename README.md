# currencyWebsite

Link for Website: https://amethyst-donica-78.tiiny.site/

I chose to create a website that uses HTML, CSS, and JavaScript to fetch
information from various APIs to convert currencies and convey information about the
currency. I wanted to create some type of application for my wild card, and I felt like doing
a website relating to currencies seemed like a great start. This website illustrates my
growth in programming and coding, which I deeply resonate with writing. I would not have
been able to write clearly and concisely at the beginning of the year, but taking this class
has helped me write better. This is the exact same thing with coding. Just like how this
class made me a better writer, my academic growth in programming has helped me learn
JavaScript, HTML, APIs, and virtual servers. Although this is a simple website, it tends to
show my growth as a programmer.

Both my portfolio’s theme and my website are deeply interconnected, as both of them are
fundamentals of software development. I set up my portfolio as a cloud terminal because it
is where I could design websites and applications. Terminal is how I can communicate with
my virtual server, an EC2 instance that is hosted somewhere else. Using the virtual server
and the terminal commands, I can construct and deploy any applications that I make. I am
not hosting my website in an EC2 instance (as it requires setup and compute time costs
money). I am using a third-party server (Tiiny Host) to host my static website.

Information about the website: After clicking on the website link provided, please wait a
moment (until the loading icon in the tab goes away) before doing anything to the website.
You can select the currencies that you want to convert from and convert to from the drop-
down menu and can input the amount you want to convert in the text field. After you click
convert, you will be able to see the converted currency(rates may not be as accurate as
the database does not update in real time). The first column will give you a list of countries
(if there are any) that use the currency. The second column should give you a graph of the
absolute percent differences between your conversion currencies from April 22-29 of
2025. You might ask, why absolute percent differences? I am sorry to say that the graph
API does not allow for negative values or for values larger than 100, so I have to structure
my graph based on absolute percent differences. The third column will show you Google
Maps of the first country displayed in the first column. You can zoom in and out of the
graph to look at and explore the country. I have the free plan for all of the APIs because
additional requests require money, so inconsistencies in the app are most probably caused
by APIs reaching their limit or fetching the wrong data.

How I made it: I used 5 APIs to create this app. The front end is coded using HTML/CSS. I
combined it with JavaScript to make this app functional. The first API gets your input values
and converts currency. Then, the second API gets all the countries that use the currency.
The responses are parsed using JS so only certain details about the country are shown.
The third API gets time series data for the currency exchange rates. Then, I compute the
percent difference for the data and store it in an array. The fourth API is the chart API,
which takes in the percent difference array and other parameters(such as graph name,
dates, and min/max values) to compute the graph. The fifth API is the Google Maps API that
lets me embed an iframe in my app. This is an overview of how I coded the website.
Apologies for the simple user interface, as I am not that good in HTML and CSS.
