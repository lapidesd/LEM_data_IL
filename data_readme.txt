This dataset contains 13 folders (MOVIE_SXX_data) of raster data that correspond to 39 animations (.mp4 and .wmv files), which show 13 different simulations of landscape evolution using lateral erosion.
Additionally, there is a folder that contains corresponding simulations using a landscape evolution model without lateral erosion (LEM-woLE_simulations), see readme within this folder.

FOLDER CONTENTS:
>2000 .asc raster files: In this data, moving down the rows is the x-direction, and moving right along the columns is the y-direction.
>1000 .jpg files showing the slope vs. drainage area relationship
>3 corresponding movie file in .mp4 format (movies_mp4_format) VLC media player on most operating systems can be used to watch these animations (https://www.videolan.org/vlc/index.html)
>3 corresponding movie file in .wmv format (movies_wmv_format) Windows media player can be used to watch these animations

For each landscape evolution simulation, we generate 1000 rasters of both elevation and drainage area of the landscape. Each raster contains 100 x 100 cells, and each cell is 150 x 150 meters.
Elevation [meters] at each cell represents the height of the landscape surface. Elevation is the greatest near the ridges and smallest in the river valleys.
Drainage area [meters squared] represents a contributing area that is upslope of each cell. Drainage area is the greatest in rivers valleys and the smallest near the ridges.
Change in elevation [mm/yr] represents how much the landscape changes over a 200 KYR window.
The number in the raster's filename corresponds to a time during the simulation. Rasters were saved at an interval of 200 KYR. Time = filename# x 200KYR.

To generate this data, we used a landscape evolution model that simulates both vertical and lateral incisional processes (https://github.com/jeffskwang). The lateral erosion component can also be found in Landlab (https://github.com/landlab/landlab).
Unless state otherwise, the following parameters were used to generate the dataset:
uplift, U = 1 mm/yr
vertical erodibility constant, K = 5x10^-5 yr^-1
stream power incision model exponent, m = 0.5
stream power incision model exponent, n = 1.0

The movie captions are as follows:
Movie S1. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Sinusoidal channel w/o random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S2. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Inclined with small perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S3. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Inclined with large perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S4. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: V-shaped valley w/ random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S5. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Sinusoidal channel w/ random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S6. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Sinusoidal channel w/o random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 0.25.  
Movie S7. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Sinusoidal channel w/o random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 0.5. 
Movie S8. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Sinusoidal channel w/o random perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 0.75. 
Movie S9. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Flat with perturbations. Boundary Condition: 1 open boundary at the bottom of the domain, and 3 closed boundaries elsewhere. KL/KV = 1. 
Movie S10. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Flat with perturbations. Boundary Condition: 2 open boundaries at the top and bottom of the domain, and 2 closed boundaries on the left and right sides. KL/KV = 1. 
Movie S11. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Flat with perturbations. Boundary Condition: 4 open boundaries. KL/KV = 1.
Movie S12. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Flat with perturbations. Boundary Condition: 4 open boundaries. KL/KV = 1. The length of the domain is 50% shorter then the simulation featured in Movie S11.
Movie S13. 200 MYR (1,000 RUs eroded) simulation showing the elevation (a), logarithm of drainage area (b), and change in elevation (c). Initial Condition: Flat with perturbations. Boundary Condition: 4 open boundaries. KL/KV = 1. The length of the domain is 50% longer then the simulation featured in Movie S11.