# Bid proposal

Customized San Francisco Basemap for Chinatown Community Development Center

<p align="left">
  
From

Yi Zhou, 
School of Architecture, Carnegie Mellon University

4919 Frew St, Pittsburgh, PA 15213

March 25, 2023

<p align="right">
To
</p>
<p align="right">
Chinatown Community Development Center (https://www.chinatowncdc.org/)
</p>
<p align="right">
(Main Office) 615 Grant Avenue, San Francisco CA 94108
</p>
<p align="right">
(415) 984-1450
</p>

  
# Timeline*: 
| Task | Time | Cost | Actual time
| --- | --- | --- | --- |
| Generate a custom palette | 0.5 | 50 | 0.5 |
| Build custom map using the Google Map Styling Wizard | 2 | 200 | 3 |
| Copy the JSON file | 1 | 100 | 0.5 |
| Lookup table | 1 | 100 | 1.5 |
| Screenshoot of the map| 0.5 | 50 | 0.5 |
| Design intentions | 1 | 100 | 1 |
| HTML page deployent | 1 | 100 | 0.5 |

*Assume a $100 per hour cost

Estimated by: Yi Zhou

Overall estimate time is 7 hours while the actual hours used are 7.5 hours. The main difference is the time used to build the google map style as the color settings can be overwritten in the geometry sublayers which result in conflict sometimes. Lookup table and screenshots are created and captured as the final step, summarizing all the design changes to the defauly map style which took longer than estimated. However, the json file and webpage deployment process are less complicated than expectation 

# Background research
The Mission of the Chinatown Community Development Center is to build community and enhance the quality of life for San Francisco residents. CCDC(Chinatown Community Development Center) is a place-based community development organization serving primarily the Chinatown neighborhood, and also serve other areas including North Beach and the Tenderloin. CCDC is a community development organization with many roles - as neighborhood advocates, organizers and planners, and as developers and managers of affordable housing. Program Teams include Community Planning, Organizing, Civic Engagement, Resident Services, Youth Leadership--all work together to build up communities, envisioning neighborhoods that celebrate empowerment, neighborhood improvement, and positive community change.

# Generate a custom palette
I use Canva's color palette generator to generate my color palatte based on one of the pics from CCDC social housing projects.
![colorpalatte](https://user-images.githubusercontent.com/79752672/227689759-16d91319-3678-4712-b0a4-5d17f3b90512.png)
* Colors from the palatte are not the final colors for customized maps, I change the RGB to increase contrast for better legibility.

# Build custom map using the Google Map Styling Wizard
Below are my customized maps for CCDC zooming in from the country level to a street level:
![scale0](https://user-images.githubusercontent.com/79752672/227696114-259588ec-0d23-441d-9a37-1a1c5575e7a2.png)
From this scale, important cities and state names are the most straightforward information. As CCDC is currently based in San Francisco, this country level gives the users a brief idea of its location in the United States. 
![scale1](https://user-images.githubusercontent.com/79752672/227696117-15eb7298-c097-44ea-baad-1926fdef80e7.png)
Zooming into San Francisco, adjacent cities such as Daly City, San Jose, Berkeley etc are shown: the human-made and landscape environment are differciated by grey and white. As CCDC is developing youth and social housing program for the Asian American population, it's important to hightlight the built environment.  
![scale2](https://user-images.githubusercontent.com/79752672/227696115-906e32e3-eac3-4ed0-9732-d081324db15d.png)
Zooming into the neighborhood scale, the street patterns become visible as well as the places of interst and transit station. Colors are aligned in order to match the design of CCDC website, icons of less important features(landscape) are hidden for legibility and clearness.
![scale3](https://user-images.githubusercontent.com/79752672/227696516-d802217b-aefd-49da-b233-944ac750be2d.png)
Going down to the street level, property outlines are visible which are important for CCDC to develop housing/voluntary/youth training programs.

Below is the lookup table that documents the feature type, element type and stylers for all relevant features which help navigate where to make changes. I go beyond the template and add more colors for contrast and gradient in transition between scales.
| Feature type | Element type | Stylers |
| --- | --- | --- |
| All | Labels / Text fill | Color: Japonica(#616161) |
| All | Labels / Text outline | Color: White(#F5F5F5) |
| All | Geometry  / Stroke | Color: White(#F5F5F5) |
| Administrative | Labels / Text fill | Color: Japonica(#B73A24) |
| Administrative | Labels / Text outline | Color: White(#F5F5F5) |
| Administrative | Icon | Visibility: Hidden |
| Land parcel | Geometry  / Stroke | Visibility: Hidden |
| Landscape | Icon | Visibility: Hidden |
| Human-made | Geometry  / fill | Color: Japonica(#E8E8E8) |
| Human-made | Geometry  / Stroke | Color: Japonica(#999999) |
| Points of interest | Geometry  / Fill | Color: Kabul(#EBCCAD) |
| Points of interest | Labels / Text fill | Color: Whitw(#757575) |
| Attraction | Geometry  / Fill | Color: Japonica(#E2A26E) |
| Park | Geometry  / Fill | Color: Kabul(#E5E5E5) |
| Park | Labels / Text fill | Color: Whitw(#9E9E9E) |
| School | Geometry  / Fill | Color: Japonica(#E2A26E) |
| Road | Geometry  / Fill | Color: White(#ffffff1) |
| Road | Icon | Visibility: Hidden |
| Highway | Geometry  / Fill | Color: Japonica(#DADADA) |
| Highway | Labels / Text fill  | Color: Kabul(#616161) |
| Station | Geometry  / Fill | Color: Whitw(#B8B8B8) |
| Water | Geometry  / Fill | Color: Whitw(#c9c9c9) |
| Station | Text  / Fill | Color: Whitw(#9e9e9e) |

# How to deploy this map?
The client can easily deploy the map style by downloading the json file here: https://github.com/xxxidragons/Zhou_portfolio/blob/bd80a5d27252d9e681681b0f692ddd78a4f80461/CCDC_mapstyle.json 
1. In the Google Cloud Console, go to the Map Styles page.

2. Click Create style.

3. Under Create your own style, select the Import JSON radio button.

4. Paste your valid JSON styling code into the field.
If your JSON is invalid, you see a notice in capital letters just below the JSON field.
If your JSON is valid, you see a preview of the pasted style, and the blue SAVE button is available.

5. Select SAVE.

The style is automatically published, and you are taken to your new style's main page.
See more details at: https://developers.google.com/maps/documentation/cloud-customization/map-styles#create-new-style 

