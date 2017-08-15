# GTM_specificscrolled
Measure if the specific area on page has been scrolled or not

Scroll Measure is one of most important and basic tracking on Google Tag Manager.
Most of methods focus on measure % of how deep users scrolled.

However, if we want to know whether a specific area is been read or not,
% tracking will be difficult to figure it out.

Therefore, we need to track based on if the class/id of the area has veen inviewed or not. 

I've write the whole steps of scroll tracking here : http://7gorange.com/2017/08/15/gtm_specificscrolled/

*I wrote it in Japanese, not sure if I have time to rewrite it in English.

To finish the tracking, you need to create a customer HTML Tag on Google Tag Manager.
Here is the Javascript code that you can copy and put it into your customer HTML Tag.

This code is been revised from Mr.Zuk whose orginal code is here : https://github.com/zuk/jquery.inview
Mr.Shimizu Makoto helps me to revise the code from Mr.Zuk.
Thanks for them.

*If I infringement anyone's patent right, please let me know and I will delete this.

The difference between this code and Mr.Zuk's code is :
It is possible to tracke several different areas at a same time.

This code is also very good because :
1. It added timer on it so that you can appoint how long you want the users to read your content.
2. The tag won't be triggered if it has already been triggered so that you don't need to worry about if it would be double counted.

Hope this code is helpful.
Leave me a message if you have any questions.
