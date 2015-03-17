# Contributors #

Open source is a wonderfull thing to connect creative minds to create new stuff for the community.

They like to share there experience and enable other to take there idea to make even better or different things.

Exactly this happend on this project :-).

|     **Who**                                                             |        **What**                                                              |
|:------------------------------------------------------------------------|:-----------------------------------------------------------------------------|
| Massimo Banzi und David Cuartielles                                   | [Adruino](http://www.arduino.cc/)                                           |
| Simon Chambers                                                        | [rx5808 SPI driver](https://github.com/simonchambers/fs-5.8g-vrx)           |
| Myles Metzel                                                          | [TVOUT](http://code.google.com/p/arduino-tvout/)                            |
| [Johannes Hermen (der-frickler)](http://der-frickler.net/)             | 5.8GHz Scanner with all above                                              |
| [Peter Blos](http://fpv-community.de/member.php?13465-pete1990)         | Simple key control + search                                                |
| [Joerg Reisener](http://fpv-community.de/member.php?384-jreise)           | Nice pictures for the SPI patch of rx5808                                  |
| [Marko Hoepken](http://fpv-community.de/member.php?14211-markohoepken) | Code optisation, TV Gui rework, distribution and maintainence of this page |

## How it started or the full story ##

Since there are more and more 32 channel 5.8GHz modules available a disscussion started in the [fpv-community.de web page](http://fpv-community.de/showthread.php?48932-32-Kanal-Videoempf%E4nger).

The most common receiver do support only 8 channels in on band (See reference).

At the bottom line it has been found that a very common rx5808 module can be controlled by an SPI bus to get all 32 channels.

It exists alreay a simple driver for [arduino](http://www.arduino.cc/) by [Simon Chambers](https://github.com/simonchambers/fs-5.8g-vrx).

[Johannes Hermen (der-frickler)](http://der-frickler.net/) took a arduino and came to the great idea to add a [TVOUT of Myles Metzel](http://code.google.com/p/arduino-tvout/).

By this he created great visual spectrum analyzer.

<a href='http://www.youtube.com/watch?feature=player_embedded&v=sQRryOsAFMg' target='_blank'><img src='http://img.youtube.com/vi/sQRryOsAFMg/0.jpg' width='425' height=344 /></a>


After a short time [pete1990 (Peter real name?)](http://fpv-community.de/member.php?13465-pete1990) took the code of [Johannes Hermen (der-frickler)](http://der-frickler.net/) and added a two button control and a simple scan search.

<a href='http://www.youtube.com/watch?feature=player_embedded&v=CqwSNj1wZtI' target='_blank'><img src='http://img.youtube.com/vi/CqwSNj1wZtI/0.jpg' width='425' height=344 /></a>


Great!

At that time I have been facinge exact the 32 channel issue since I bought a new TX module.

I found the artice [about the 32 channel RX in the fpv-community.de web page](http://fpv-community.de/showthread.php?48932-32-Kanal-Videoempf%E4nger).

The existing code at that time was in the state of early prototype.

My part has been refactoring and cleaning the code up first.

From there code optimisation in the driver and tune handing reduced the
full 32 channel time from 10 t0 1 second (!).

I loved the [TVOUT of Myles Metzel](http://code.google.com/p/arduino-tvout/) an experimented with it.

By using a screen of 128x96 pixel it was possible to improve the naviation an give nice informative screens.



<a href='http://www.youtube.com/watch?feature=player_embedded&v=fjriVj_pkpU' target='_blank'><img src='http://img.youtube.com/vi/fjriVj_pkpU/0.jpg' width='425' height=344 /></a>

Finally I put all this on this code.google page to have all together for the world wide comunity of builders.

Thanks to all, Marko Hoepken