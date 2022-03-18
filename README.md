# OptimAdvAllocations

Assume we have an optimised set of ads served (impression) to the user on a given device at the **(days,campaign,geogroups)** level - how do we assign this at the **postcode (geokey)** level. The geogroup can be thought of as a **Postcode Sector**.

Notebook contains some ideas for distributing geogroup (Postal sector) to geokeys (postcode) as integer values. Essentially an **integer optimisation problem**.

Some assumptions:

* There are around **1.4 million postcode geokeys**
* Around **10k** postal sectors (geo groups).
* We cannot have **fractional impressions**, so have consider approaches such as the **D'hondt method**.

