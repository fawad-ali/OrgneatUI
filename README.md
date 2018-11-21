# OrgneatUI
A simple .net based project, based on Twitter Scraping principal to download historic Tweets. This project has standard library and UI. Library can be imported to any other projects. UI is a demo and quick use tool.

# For basic instructions and Screen shots, for now please visist this page: http://www.orgneat.com/Request

# Highlight

There are many Python and Java based programs on Github. My own program is inspired by great work others have done, especially GetOldTweet program by Jefferson Henrique. This program is just an attempt to make it easy way for users to download tweets without engagging into Python learning or setting up enviornment.

The .Net code is although not Commercial grade, but pretty much close that consider lot of different scenarios such as what if Twitter do not respond, if there any timeout, if there is any issue with Tweet html etc.

One of the reason behind making GUI is ease of use. Although the library behind it in Collector folder can support consle application. The GUI makes it lot easier to provide a way to enter advanced queries without worrying about how to configure the parameters.

Based on my experience Python on my local computer takes lot of Memory and Processor. I did multi threading on Python and each thread would take at least 200 MB memory. .Net code is pretty efficient in memory handling and processor scheduling. Upon testing, even for 20 threads, program would take less than 50% Processor (Intel core i7 4th Gen) and about 500 MB in total memory. This reduces time required to download millions of tweets without compromising performance.

If you feel this code is worth taking your attention, please try it once, feel free to contribute as well.

Following are some screenshots.
Main query window: Specify your query in this window.
  
Stats window: Once you fill in the form and click on Yellow button, without saving any tweets, this window will show you stats about your query. whether will it work, and if it works how much time will it take to download etc.
  
Process window: Once you are done filling form and select number of threads you want to start then select folder to save, click on Start button. This window opens with all threads running, live stats and shows you how many tweets have been downloaded.
  
Some of the basic instructions:
Fill in all required fields as you want. Please make sure you enter correct words. I haven’t tested all fields yet. Also remove word button may not work. Sorry the UI is work in progress.
Select dates, language and/or Location. For location please refer Twitter, how to enter locations. You can choose within field or leave it 0.
Next, click Save Folder button to select where you want these files to store.
Next you can click on Yellow button to test it out. You don’t have to, but I would suggest see the stats and try the query first.
Next from “Parallel threads” dropdown list, select number of threads you would like. Threads are the parallel scraper that divide your query in number of parallel processes to speed up entire process. Sometimes one query can take days to collect all required tweets. Dividing them speeds it up. Also it pushes processor to its limit so that’s why I have restricted the number to 20.
Finally click on start process button. It will open a new window with logs and stats of threads. You can keep it running.
