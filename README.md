# InfiniteProsCustomsData
A repo containing the work I did to scrape, ingest, and explore Halo Infinite stats

I can add some of the scripts I made to download and put these games into a database if people really want, but why I'm releasing this is because it largely stopped working and required too much upkeep. I used a combination of HaloDotAPI and HaloTracker requests at first, then I switched over to Autocode with HaloDotAPI, and now they're shutting down and asking for money instead of just open sourcing what they re'd, so I'm not expecting a reliable and stable way to get match stats for Halo Infinite anytime soon. I get things cost money, that's why I turned off SpartanFinder.com, but open sourcing things allows anyone to come in an contribute. 

So here's the database I maintained with games from 11/15/2021 to 5/4/2022. It contains match stats from custom games largely between Pros. Obviously there's a fluid definition of who counts as a Pro but I maintained a list of players who where either on partnered teams, or on the top teams in their region (yes I tried to get players from all regions). The scraping process didn't discriminate so basically if an Infinite Pro played in a custom game, it ended up in here. So I certainly recommend filtering down to the games you care about before doing any analysis.

What I ultimately used this for was to create an RAPM or regularized adjusted plus-minus metric for Halo players. I did this by game type, and rolled it up into a game predictions model that only worked okay. It clearly had some issues like not suppressing non-NA players because they disproportionally played poorer competition (as in they played people in their region more). I have a path forward with it, but the game's general interest has cratered and I don't think it would be worth my time to build one either from either a betting or integrating-into-the-scene perspective. 

So here's a database file with what I had, everything should be fairly self explanatory. At some point along the way medals were parsed out so a second table was created to store those for games that had them. If you download this and do something with it, let me know! If you have any questions or comments, let me know! Just open up an issue ticket here or message me on discord: CYRiX#5864
