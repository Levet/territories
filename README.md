Risk inspired game using D3.
=========================

This is mainly just to get a better understanding of d3 capabilities, and interweaving classes with d3 elements.

Challenges
=========
1: Dynamically finding bordering "territories" base off of shared coordinates.
- Ideally any topography could be passed in and be made into a playable map.
- On load it would find areas with shared borders and those would be "attackable" territories.

+ Filter out all coordinates that are map borders.
+ Using the first territory in the list, find a territory that borders it.
+ Mark both territories as bordering each other.
+ Remove shared coordinates from each territory's available coordinates list.
+ Move to next coordinate, until available coordinates list is empty.

2: Random territory grouping for bonus troops.
- Given an arbitrary map, grouping territories to form regions/countries/states.
- Groups should share borders
- Outliers, such as islands, should be grouped into existing groups. Unless there are more than one territory within them.
- Rewards for holding "regions" should be based off how hard it is to capture and hold.
