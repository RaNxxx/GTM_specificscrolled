# GTM_specificscrolled
This code was designed to measure the specific area on a page that has been scrolled down.

Scroll Measure is one of most important and basic tracking meters on Google Tag Manager.
Most of methods the focus on measuring the percentage of how deep users scroll.

However, if we want to know whether a specific area has been read or not,
it will be difficult to figure out with % tracking.

Therefore, we need to track based on if the class/id of the area has been in view or not.

I have written all of the steps of scroll tracking here : http://7gorange.com/2017/08/15/gtm_specificscrolled/

*I wrote it in Japanese, not sure if I have time to rewrite it in English.

To finish the tracking, you need to create a custom HTML Tag on Google Tag Manager.
Here is the Javascript code that you can copy and put into your custom HTML Tag.

This code has been revised from Mr.Zuk whose orginal code is here : https://github.com/zuk/jquery.inview
Mr.Shimizu Makoto helps me to revise the code from Mr.Zuk.
Thanks to both of them.

*If I infringe anyone's patent right, please let me know and I will delete this.

The difference between this code and Mr.Zuk's code is :
It is possible to tracke several different areas at a same time.

This code is also very good because :
1. It added a timer on it so that you can appoint how long you want the users to read your content.
2. The tag won't be triggered if it has already been triggered so that you don't need to worry about if it would be double counted.

Hope this code is helpful.
Leave me a message if you have any questions.
