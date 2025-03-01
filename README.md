# Russia-Ukraine War

Using data from [Oryx's site](https://www.oryxspioenkop.com/2022/02/attack-on-europe-documenting-equipment.html), I've put together a quick tracker to visualize equipment losses since [Russia's February 24th invasion of Ukraine](https://en.wikipedia.org/wiki/Russo-Ukrainian_War). This is only equipment that is independently verified, as noted by Oryx:

> This list only includes destroyed vehicles and equipment of which photo or videographic evidence is available. Therefore, the amount of equipment destroyed is significantly higher than recorded here. Small arms, munitions, civilian vehicles, trailers and derelict equipment (including aircraft) are not included in this list. All possible effort has gone into discerning the status of equipment between captured or abandoned. Many of the entries listed as 'abandoned' will likely end up captured or destroyed. Similarly, some of the captured equipment might be destroyed if it can't be recovered. ATGMs and MANPADS are included in the list but not included in the ultimate count. The Soviet flag is used when the equipment in question was produced prior to 1991. 

Data is drawn from [this public google sheet](https://docs.google.com/spreadsheets/d/1bngHbR0YPS7XH1oSA1VxoL4R34z60SJcR3NxguZM9GI/edit?usp=sharing) which is updated based on the last update for each day. As such it is a lagging indicator, dependent not just on when equipment is lost, but when it is discovered and documented. 

Data is pulled daily from Oryx's site using [Daniel Scarnecchia](https://github.com/scarnecchia)'s [scraper tool](https://github.com/scarnecchia/scrape_oryx), and then pushed to the public google sheet, where synthetic calculations are performed for equipment categories (to presere transparency). 

Points (red = Russia, blue = Ukraine) represent cumulative losses for each day, bar's represent daily losses. The line repreents a general additive model smooth on cumulative losses to date; the shaded grey band represents the 95% confidence interval based on extant variation (e.g. point scatter). A wider grey band means more uncertainty, a narrower grey band means less uncertainty. 

Please keep in mind that this is empirical, not inteptetive, analysis. A concern raised about the available data is that it undercounts Ukrainian losses. This is possible not just because of bias (note pro-Russian sources are monitered as well) but because areas under Russian control are less likely to have photo documentation. Fog of war is very real. There is no attempt here to use a modifier to adjust numbers - analysis is strictly empirical. Any bias in the origional data will be reflected in the following analyses.

## Total Equipment Losses
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_total.jpg?)
Ukranian and Russian equipment losses started off equivalent, but Russians quickly began to lose more equipment by the third day of the war. 

## Destroyed Equipment
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_destroyed.jpg?)
Destroyed Russian equipment outpaced destroyed Ukranian equipment by the second day of the war, though there are signs it is starting to taper. 

## Abandoned Equipment
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_abandoned.jpg?)
Ukranians abandoned equipment more readily in the early days fo the war, but by the third day this rate plateaued. Russian abandonments increased sharply on the third day, and began to taper at the end of the first week.

## Captured Equipment
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_captured.jpg?)
Russians have seen a much higher rate of equipment capture since the start of the war, with a sharp increase in the second week, though this has begun to taper by the start of the third week. 

The degree to which Russians have lost more equipment (in every category type) is very striking. It is certaintly possible this is a product of Ukranians focusing on documenting Russian losses, though this can't be a complete explanation. 

## Equipment Net Changes
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_absolute_total.jpg?)
This calculation subtracts units captured by each combatant with their other loss types (destroyed, damaged, and abandoned). It is arguable if a proportion of abandonded should be included as captures. Ukraine has a net positive change in equipment - meaning they've captured more than they've lost. Russia however has lost many more units than it has aquired from Ukraine. 

## Ratios
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/ratio_grid.jpg?)
This plot shows the ratios of losses (e.g. proportion of total) for Russia and Ukraine for each loss type.  

# Refugees
These data are gathered by the United Nations High Commissioner on Refugees (UNHCR) operational data portal (ODP) [here](https://data2.unhcr.org/en/situations/ukraine). The line represents total refugees, while the bars below indicate daily totals. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/refugees_total.jpg?)

Refugee outflows peaked on the 7th of March, but migration continues to be heavy. Refugees are primarily destined for Poland initially, though other nearby countries such as Moldova and Hungary are taking large numbers as well. This only counts migration out of Ukraine - internal displacement of [7.1 million people](https://displacement.iom.int/reports/ukraine-internal-displacement-report-general-population-survey-round-2-24-march-1-april) has occured since the conflict began. All together over 25% of Ukraine's population, or more than 1 out of every 4 Ukrainians, has had to move since the war began. 



# Raw Equipment Losses
"Raw" refers to a specific type of vehicle, such as a tank or armored personell carrier

## Tanks
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_tanks.jpg?)
Tank losses were equivalent in the first four days of the war, with Russian tank loses increasing sharpely thereafter, though a jump in Ukranian tank losses can be seen at the start of the second week of the war. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_total_tanks.jpg?)
This graph, however, highlights the challenges Ukraine still faces. When the sheer scale of [Russian tanks](https://inews.co.uk/news/world/russia-tanks-how-many-putin-armoured-forces-ukraine-nato-explained-1504470) are considered (13,300 vs. 2,100 for Ukraine), the steep Russian losses are not yet bringing parity. In general, Ukraine loses 1 tank for every 3 it takes from Russia. This ratio has to get to 4 or higher to be sustainble. Note that this estimate factors in verified tank captures by both Russia and Ukraine. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_deployed_tanks.jpg?)
If we consider estimates of [deployed Russian tanks](https://en.as.com/en/2022/02/24/latest_news/1645729870_894320.html) instead of their total (2,840 vs. 2,100 for Ukraine), the picture is not as dire for Ukraine. This estimate likely is closer to the battlefont picture, as not all Russian tanks could be deployed at once, though Russia can sustain attrition longer than Ukraine. Note that this estimate factors in verified tank captures by both Russia and Ukraine. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_total_tanks_baseline.jpg?)
If we consider estimates of [deployed Russian tanks](https://en.as.com/en/2022/02/24/latest_news/1645729870_894320.html) fixed to their total inventory, it is clear that Ukraine is adding to its tank fleet near the rate Russia is losing theirs. Though note that this measure assumes Russia has the capability to use all 13,300 of its tanks in Ukraine if needed. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_deployed_tanks_baseline.jpg?)
If we consider estimates of [deployed Russian tanks](https://en.as.com/en/2022/02/24/latest_news/1645729870_894320.html) fixed to their starting number, the picture is considerably more positive for Ukraine. Instead of recording only losses, this fixes the baseline (2,840 for Russia vs. 2,100 for Ukraine) and factors both tank losses and gains (e.g. captures). By this metric Russia has lost well over 5% of its tanks while Ukraine has supplemented its by 2% (e.g. captured more than it has lost).



## Armored Fighting Vehicles (AFV)
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_afv.jpg?)
Armored Fighting Vehicles also see parity in losses in the first 4 days of the war, though Russian losses increase less dramatically than is seen with tanks. Note that this estimate factors in verified AFV captures by both Russia and Ukraine. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_afv.jpg?)
When normalized to standing inventory, Russia's losses are a less significant fraction of their total inventory compared to Ukraine. This higlhights the steep challenge Ukraine faces. In general, Ukraine loses 1 AFV for every 3 it takes from Russia. This ratio has to get to 4 or higher to be sustainble. 

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_total_afv_baseline.jpg?)
If we consider estimates of [deployed Russian AFV](https://en.as.com/en/2022/02/24/latest_news/1645729870_894320.html) fixed to their total inventory, Ukraine is adding modestly to its AFV inventory at the same rate which Russia is losing its AFV. 

## Infantry Fighting Vehicles (IFV)
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_ifv.jpg?)
Ukranian's lost more Infrantry Fighting Vehicles in the first two days of the war, with Russian losses acellerating linearly until the end of the second week. 

## Armored Personel Carriers (APC)
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_apc.jpg?)
Ukranian's lost more Armored Personel Carriers in the first two days of the war, with Russian losses acellerating linearly until the end of the second week, though the differential is less dramatic than with AFVs.

## Infantry Mobility Vehicles (IMV)
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_imv.jpg?)
Infantry Mobility Vehicle losses are more or less equivalent between Ukranian and Russian forces through the first two weeks of the war. 

# Synthetic Equipment Losses
"Synthetic" refers to a combination of vehicle types to form a theme - such as aircraft (fighters + helicopters + drones) or anti-aircraft (SAM + MANPADS), etc. 

## Aircraft
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_aircraft.jpg?)
Ukranians have lost aircraft linearly, while Russians lost them almost exponentially in teh first two weeks of the war, though there are signs this is tapering sharpely. This calculation includes fighters, helicotpers, and drones. 

## Anti-air
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_antiair.jpg?)
Ukranians sustained higher rates of loss of anti-air systems through the first week of the war, though Russian losses have since outpaced them by the second week of the war. This calculation includes MANPADS, SAMs, self-propelled anti-aircraft guns, radar, and jamming systems. 

## Armor
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_armor.jpg?)
Russian and Ukranian armor losses were equivalent in the first three days of the war, with Russian losses significantly outpacing Ukranians since. This calculaton includes both tanks and armored fighting vehicles.

![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_percent_total_armor_baseline.jpg?)
If we consider estimates of [deployed Russian armor](https://en.as.com/en/2022/02/24/latest_news/1645729870_894320.html) fixed to their total inventory, Ukraine is adding modestly to its armor inventory at the same rate which Russia is losing its Armor. 


## Infantry
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_infantry.jpg?)
Infantry losses were higher among Ukranians at the start of the war, with Russian losses increasing sharply since then. Ukranian losses taper in the second week. This calculation includes infantry fighting vehicles, armored personell carriers, and infantry mobility vehicles.

## Vehicles (standard transportation)
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_vehicles.jpg?)
Ukranians lost more vehicles on the first day, with Russian losses accelerating since then. This calculation includes all non-specialized vehicle types. 

## Logistics Systems
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_logistics.jpg?)
Ukranians have lost few logistics systems, while Russian losses increased linearly until the end of the second when they began to taper. This calculation includes engineering and communications vehicles.

#Analysis
By grouping synthetic vehicles, we can see how different systems have been prioritized by Russian or Ukranians, providing a glimpse into strategy. 

## Loss Type
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_loss_type.jpg?)
These ratio plots use Russian equipment losses as the numerator and Ukranian losses as the denominator. The higher the bar, the higher the proportion of Russian losses. While Russians have abandoned vehicles at a higher rate, destructions remain the highest differential between the two armies. 

## Unit Type
![alt text](https://raw.githubusercontent.com/leedrake5/Russia-Ukraine/master/Plots/current_unit_type.jpg?)
Here, Ukranian strategy is abundantly clear. It has targeted Russian logistics operations (higher bar = more Russian losses) to an overwhelming degree. Russians have focused on anti-air systems (lower bar = more Ukranian losses), though remarkably despite this focus Ukranian's still have an almost 2-1 edge on taking these systems out. 

# Conclusions

I am not a military expert, but by the second week of the war it is clear that the Russian objective of suppressing Ukranian aircraft and anti-air failed, leading to contested airspace. In contrast, Ukranian's succeeded in interfering with Russian logistics, evidenced by their focus on logistics vehicles and fuel lines. This has ground the Russian advance to a halt by the third day, with limited change since then. 
