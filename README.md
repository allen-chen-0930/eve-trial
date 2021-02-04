[1] Introduction
Eve helps users identifying trend patterns and their fibonacci levels. Once the current price is approaching one of the fibonacci levels, Eve would tell users about it from the left-top side panel in the mql5 terminal and their phones.

[1.1] Introduction Into Details-Settings (Options)
Please read this paragraph with the gif url below, [https://media.giphy.com/media/EKzs0itqWzvkdeMreH/source.gif].
Before turning on Eve, you need to check some settings. Open up the Options dialog (Tools->Options), then check these two tabs, Expert Advisors and Notifications.
In the Expert Advisor tab, add two urls into the Web Request List, "http://zfold.net" and "zfold.net" then click the following check boxes (Allow DLL Imports, Allow WebRequest for listed URL).
In the Notifications tab, do make sure the two check boxes checked and your MetaQuoteIs Id typed in (Enable Push notifications, Notify of trade transactions). 
Click the “OK” button after the above things done.


[1.2] Introduction Into Details-Settings (Eve)

Please read this paragraph with the gif url below, [https://media.giphy.com/media/DhPkQNYkccZ0hdzucs/source.gif]. 

Before turning on Eve, you need to check some settings. Open up the Eve dialog then check the first tab, Common tab.

In the Eve Trial Version, only EURUSD symbol is available. Eve Trial Version would be auto-shut down once

it's attached to any other symbols rather than EURUSD.



Click the Inputs tab, several input variables would be listed shown below.

--------------------------------------------------

[1] Bar Start At (Fibonacci)

Define the start bar while re-calculating the fibonacci levels. "0" stands for the current bar.

[2] Bar Back To (Fibonacci)

Define the last bar while re-calculating the fibonacci levels. 

[3] Bar Back To (Zigzag)

Define the last bar while re-calculating the zigzag patterns.

[4] Coef. of PER (Zigzag)

"Coef. of PER" means the "Coefficient of Price Extreme Range". 

The smaller the value, the more sensitive zigzag patterns would be.

[5] Back Step At (Zigzag)

Define the start bar while re-calculating the zigzag patterns.

[6] Enable Notice

Set it as true, users would get notifications from their phones.

[7] Notice Timer (ms)

Define the timer of notice in milliseconds.

--------------------------------------------------

You could adjust there input variables on your own or just leave them with default values.

[1.2] Introduction Into Details-Panel/Chart/Notice
Please read this paragraph with the gif url below.
[https://media.giphy.com/media/jgbzR8Psr0c3BOL8do/source.gif]
After Eve turned on, you could see how it work like the gif url listed above.
[1.2][Panel]
The introduction would start from the left-top side panel. Please read the following content.
*********************************
[TREND]->UP/NONE/DOWN
PS= Tell user what the current trend is (UP/NONE/DOWN).
[SLOPE]->NUMBER
PS= More detailed [TREND], tell user its slope.
[FB-LV-7]->NUMBER
PS= Display the price at level 7 of fibonacci.
[FB-LV-6]->NUMBER
PS= Display the price at level 6 of fibonacci.
[FB-LV-5]->NUMBER
PS= Display the price at level 5 of fibonacci.
[FB-LV-4]->NUMBER
PS= Display the price at level 4 of fibonacci.
[FB-LV-3]->NUMBER
PS= Display the price at level 3 of fibonacci.
[FB-LV-2]->NUMBER
PS= Display the price at level 2 of fibonacci.
[FB-LV-1]->NUMBER
PS= Display the price at level 1 of fibonacci.
[FB-LV-0]->NUMBER
PS= Display the price at level 0 of fibonacci.
[C-PRICE]->NUMBER
PS= Display the current price.
PS2= Order ([FB-LV-7]~[FB-LV-0]~[C-PRICE]) would be changed dynamically based on the computation.
*********************************
[1.2][Chart]
After the left-top side panel, please check the zigzag patterns (trend lines, blue + red) in the chart.
Users could get the big picture of the market trend according to the zigzag patterns.
After the zigzag patterns, please check the last part, the fibonacci levels (8 horizontal lines, blue).  
To be brief, fibonacci levels could be seen as a potential support/resistance line. 
It could be a utility as the reversal identifier.
[1.2][Notice]
Users could get notifications from their phone if the notification is turned on.
its content would be something like this,
*********************************
Eve, [EURUSD], [C-PRICE] is approaching [FB-LV-0]. [C-PRICE]=1.01, [FB-LV-0]=1.02.
*********************************

