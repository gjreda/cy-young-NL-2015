Visualizing the 2015 National League Cy Young Race
==================================================

Originally, I started digging into this data in attempt to show that Jake
Arrieta should win the 2015 NL Cy Young. However, the data showed that it was
difficult to make that case with a straight face.

Instead, I did a bunch of analysis around each of Arrieta, Greinke, and
Kershaw's seasons and made some fun plots to show how their seasons progressed.

This repo contains all the code and data for that analysis.

The article I wrote around this never got published, but here it
is in case you're interested in reading it (though it's now outdated).

-------------------------

Tonight, we’ll finally learn the winner of this year’s National League Cy Young award. The contenders -- Jake Arrieta, Zack Greinke, and Clayton Kershaw -- all had stellar years, each putting up numbers we haven’t seen in a long time. So stellar though, that making a case of why one should win over the other two is impossible to do with a straight face.

To illustrate, take a look at the chart below, which shows how some of their stats moved throughout the season. Except for Kershaw’s clear superiority when it comes to striking out hitters, every other stat is neck and neck.

![stats-comparison](/images/stats-comparison.png)

This year’s winner comes down to how the Baseball Writers of America weighed consistency against dominance and traditional stats against advanced stats.

### Jake Arrieta

If you’re not already familiar with Jake Arrieta’s record breaking second half, one look at his ERA chart above should get you up to speed quickly. His post all-star break numbers were magical, allowing only nine earned runs over 107 ⅓ innings -- good for a 0.75 ERA, the best since the All Star game became a thing in 1933. He was pretty much unhittable during that stretch -- .148 AVG, .409 OPS, and only 2 HR allowed. Oh, and he no-hit Greinke and Kershaw’s Dodgers on August 31.

The baseball traditionalists will argue that Arrieta’s major league leading 22 wins make him most deserving of the award, but those who have been paying attention throughout the last decade have learned that [pitcher wins are a pretty poor measure of quality](http://www.hardballtimes.com/lets-get-rid-of-pitching-wins/). However, when you add in that he finished second in ERA and WHIP, you’d think he’d be assured the award - and in a typical year, you’d be right.

But while Arrieta’s second half was nothing short of dominant, Greinke’s consistency throughout the season is impossible to overlook.

### Zack Greinke

Greinke’s major league leading 1.66 ERA is where his candidacy begins -- at no point during the season did his ERA even reach 2. The last time a starter post an [ERA below 1.70 was Greg Maddux in 1995](http://bbref.com/pi/shareit/MEsTK). And yes, Maddux did win the Cy Young that year.

He led the majors in ERA, ERA+ (which adjusts for ballpark factors), and WHIP, all while having a unique ability to avoid giving up extra-base hits (XBH%) and maintaining a low batting average on balls in play (BABIP).

![rates-comparison](/images/rates-comparison.png)

But this is where the argument for Greinke begins to falter. Advanced stats like BABIP and fielding independent pitching (FIP) are typically viewed as ways to measure a pitcher’s defensive luck. It’s unfortunate for his candidacy that he had the second lowest BABIP in the majors and a FIP not only higher than both Arrieta and Kershaw, but also [1.1 higher than his ERA](http://www.baseball-reference.com/leagues/MLB/2015-standard-pitching.shtml#players_standard_pitching::28).

One could argue that Greinke creates this “luck” by inducing weak contact and enabling his defense to shine, but we see evidence of the contrary in that opponents, on average, hit Greinke about 3.4 MPH harder than both Arrieta and Kershaw.

![batted-ball-exit-velocity](/images/avg-batted-ball-velocity.png)

[There’s a significant relationship](http://fivethirtyeight.com/features/chase-utley-is-the-unluckiest-man-in-baseball/) between how hard a ball’s struck and its likelihood to wind up as a hit, so it’s unexpected to see that despite being hit harder, he has the lowest BABIP and XBH% of the three.

### Clayton Kershaw

Though Kershaw’s ERA is pedestrian when compared to Arrieta and Greinke, it’s easy to argue he was the most unhittable of the three, [striking out more than a third of opponents](http://bbref.com/pi/shareit/RiFmd) -- something only Randy Johnson, Pedro Martinez, and Kerry Wood have done. Hitters only put the ball in play in 59% of their appearances against Kershaw.

Additionally, while the case for Greinke is harmed by BABIP and FIP, Kershaw’s case is helped. Despite playing on the same team and inducing weaker contact, Kershaw’s FIP was 0.77 higher than Greinke’s, indicating that he didn’t catch the same breaks (or luck) Greinke did. Kershaw’s also this year’s darling of advanced stats like WAR, with [Baseball Prospectus](http://www.baseballprospectus.com/sortable/extras/dra_runs.php), [FanGraphs](http://www.fangraphs.com/leaders.aspx?pos=all&stats=pit&lg=all&qual=y&type=8&season=2015&month=0&season1=2015&ind=0&team=0&rost=0&age=0&filter=&players=0&sort=19,d), and [OpenWAR](https://gjm112.shinyapps.io/openWAR/) all agreeing he’s the leader.

--------------------

When considering who will win the award though, it’s important to remember that the BBWAA tends to lag behind when it comes to the use of advanced statistics -- it wasn’t until recently they started accepting pitcher wins as a flawed statistic. Similarly, in the [108 Cy Youngs awarded from 1956 through 2014](http://www.baseball-reference.com/awards/mvp_cya.shtml), only 25 times has the winner not been the candidate with the lowest ERA or the most wins. For this reason, we should expect Greinke or Arrieta to win the award.

But then again, a tie [wouldn’t be unprecedented](https://en.wikipedia.org/wiki/Cy_Young_Award#American_League_.281967.E2.80.93present.29).

--------------------

#### Data sources:

- [Baseball Savant](http://baseballsavant.com/) for the PITCHf/x data

- [Baseball Reference](http://www.baseball-reference.com/) for the game logs
and historical voting data
