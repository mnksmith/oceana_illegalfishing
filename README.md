# Fighting Illegal Fishing: Global Fishing Watch and Oceana
## Background

We are facing an ocean health crisis.  Climate change, ocean acidification, pollution, and overfishing are stretching marine ecosystems to the breaking point, threatening their ability to sustainably provide food and livelihood to billions of people around the world.  Rampant overfishing has imperiled global commercial fish stock to the point that nearly 90% of the world’s fisheries are already fully exploited, over-exploited, or depleted to the point of collapse.  Illegal, unreported, and unregulated (IUU) fishing is a major contributor to this crisis, accounting for an estimated 20% of the total catch and costing tens of billions of dollars annually.  The perpetrators of IUU fishing ignore protected areas, use harmful and invasive fishing techniques, follow no standards of health and sanitation, and are often associated with other illegal activities such as forced labor and even human trafficking.

## Fighting IUU

By nature, combating IUU fishing is a formidable challenge.  It often takes place outside of governmental jurisdiction on the high seas or in the waters of developing countries that lack the resources to enforce the law.  Illegal fishing vessels change names, owners, and flags frequently, and will turn off or manipulate required tracking systems to obscure their locations.  The fish is transported by third-party reefer ships and brought to market hidden under a false species designation.  Licensing and other documentation is forged and money earned disappears behind the borders of haven countries.  Even efforts to define the scope of the problem have been confounded by this complex tangle of issues and its globalized nature.

## Oceana and Global Fishing Watch

[Oceana](https://oceana.org/) is a global ocean conservation organization based in the United States. One of Oceana's priority campaigns is combating IUU and seafood fraud ([link](https://usa.oceana.org/our-campaigns/illegal_fishing_and_seafood_fraud/campaign)). A primary partner in tracking and identifying IUU is the [Global Fishing Watch](https://globalfishingwatch.org/) (GFW), an offshoot of Oceana with a narrower mandate of sustainable fishing through transparency. GFW hosts a live map of global fishing activity, and analyzes patterns to identify suspicious patterns and locations in fishing behavior.

## ML strategies for detecting illegal fishing

### The data

The primary tool by which governments and watchdog organizations like GFW and Oceana can monitor fishing activity is vessel tracking data. The International Maritime Organization and many national governments require all vessels to carry AIS (automatic identification system). These devices automatically ping satellites with the vessel's location, primarily to avoid collisions. All told, an enormous amount of location data is available for public use, and private/secure tracking is available via government cooperation in other impactful fishing regions of the world like Indonesia. Note: though only a fraction of all fishing vessels in the world have AIS, the vessels that do are responsible for an outsized proportion of fishing volume.

### The goal

With all of this data, the hope is that a machine learning algorithm is capable of sorting through the chaos and flagging vessel tracks that look like IUU. In order to train the algorithm, GFW has had fisheries/maritime experts manually tag thousands of vessel tracks with the type of ship, its size, its type of gear, and based on those properties, whether it's fishing. Vessels exhibiting fishing behavior where it is prohibited can be quickly identified, located, and brought to the attention of authorities.

### The contents of this repo

Here you can find an example notebook for a first-pass classifier based on a logistic regression. Feel free to reach out for train/test vessel track datasets.

