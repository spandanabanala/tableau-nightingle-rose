# tableau-nightingle rose-

Image of Visualization of Nightingale dataset:



 Tool: Tableau Desktop, Tableau public
Description:
• Visualization of Nightingale:
 The nightingale visualisation was done during Crimean war it gave the details of mortality rates of
soldiers
The goal of this visualisation is to compare the mortality based on the cause of disease.
First using pivot in tableau ,converted Zymotic diseases, Wounds & injuries, All other
causes columns to rows (for both Annual rate of mortality per 1000,Deaths). And renamed the field
to cause of death.
Next we create the path field for every instance which will be used to draw to polygon slices for each
month and cause of death type.
Now we take path values as 1and 102 as we want edge of the slice to be rounded.
These paths are used to draw slice by assigning total of 102 X and Y points .Each slice is a polygon
comprised of 102 points.
Next we take polygon mode in tableau and we need to create X and Y values.
Have added month column which is of datatype date and time.
After pre-processing the data set
First create the path( bin ) column in dimension mode and make bin size 1 and continues this will be
used by the path marker to draw slices
I used below markers for marking the graph based on
colour marker for cause of death and month
Tooltip to represent values of annual rate of morality ,cause of death, number of deaths .
calculated fields that need to be created for each path
counts and indexes, which work out how many slice to draw and in turn determines the angles which
is calculated using month.
Number of slices need will be calculated using month and path(bin)
Now in order to know the X and Y values of edges of the polygon we need the angle and size,radius.
For each path id in path (bin) we calculate
Radius
X
Y
Now using year filter separated based on the range of year
Finally used dashboard and replicated the nightingale coxcomb graph

