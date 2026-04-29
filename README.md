The initial data comes from data.gov which is the official location of all open datasets published by the federal government.
Each row represents a building permit issued in DC. 
As far as I can tell the database is pruned to not include demolished buildings or lots that have since been merged, split, etc. 
The dataset draws mainly from permits issued by the city from 1877-1949. 
Additionally, examining DC’s history through building permits will inevitably highlight those with the means to buy land, architects, developers, and local officials. 
People who don’t fit those profiles may be figures worthy of study but will not through this dataset. 
My project aimed to identify historical kit houses in Ward 3, analyze their construction patterns relative to historical streetcar lines, and compare their modern-day assessed values to national and local averages. 
I expected a big boom in the 1910s and 1920s, tapering off afterward due to the Great Depression and WWII.
I also anticipated major development along public transport and the current price of these homes to be substantialy higher than their initial costs. 
The process began by filtering a dataset of over 126,000 D.C. property records to isolate the ~35,000 addresses located on Ward 3 streets. 
These addresses were processed through a geocoding API in chunks to obtain precise latitude and longitude coordinates for mapping. 
Houses were identified using two methods: searching official "Architect" fields for known kit companies and extracting the text on unstructured notes and builder fields to find hidden mentions of terms like "Sears," "Honor Bilt," or "Ready-cut".
The property records were joined with D.C. tax assessment data using cleaned "Square-Suffix-Lot" (SSL) identifiers to fetch modern financial values.
The project incorporates historical streetcar corridor data to visualize how early 20th-century transit influenced the speculative development of these pre-cut homes.
The final output includes interactive maps that use color-coding to represent the era of construction (e.g., the 1920s boom) and marker size to reflect modern assessed values, providing a visual argument for the lasting economic and architectural legacy of kit houses in D.C..
