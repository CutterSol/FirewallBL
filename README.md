This list can be added to an Asus router running Merlin via AMTM in the Skynet app.  I initially add anything I am testing via the "fast switch" option of the Skynet settings first.  Then if you have a list you like better than the default for Skynet you can update the default Skynet list with that list.  This list is actually a lists of list, when Skynet does it's update it will check for updates to each of thse list--they are dynamic and change daily.  The list can be checked at firehol.  The lists in the file (default as of 10/24) were checked for update frequency, composition, and reviews on FireHol.  Most of them have updated within the last week, don't have a lot of complaints in their reviews, and are used in other lists to provide a signifcant portion of those lists blocks.

If you want to validate your list check this repo: https://github.com/ViktorJp/FilterValidator\

Notes on FilterValidator:
wget https://github.com/ViktorJp/FilterValidator/blob/main/filtervalidator-0.7.sh 

This didn't work, so had to use FV without version number, so remove "-0.7"...  

chmod +x filtervalidator-0.7.sh 

sh filtervalidator.sh
Then give the RAW github link when prompted...  

