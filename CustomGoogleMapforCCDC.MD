# Bid document for customozed google map for non-profit organization

Client: Chinatown Community Development Center (https://www.chinatowncdc.org/)

Location: (Main Office) 615 Grant Avenue, San Francisco CA 94108

Contact: (415) 984-1450

Start date: 03/25/2023

Estimate*: 
| Task | Time | Cost | Actual time
| --- | --- | --- | --- |
| Generate a custom palette | 0.5 | 0.5 | 1 |
| Build custom map using the Google Map Styling Wizard | 3 | --- | 3 |
| Copy the JSON file | 1 | --- | 0.5 |
| Lookup table | 1 | --- | 1.5 |
| Screenshoot of the map| 0.5 | --- |
| Design intentions | 2 | --- |
| HTML page deployent | 1 | --- |

*Assume a $100 per hour cost

Estimated by: Yi Zhou

Screenshots are taken

# Background info
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
Zooming into the neighborhood scale, 
![scale3](https://user-images.githubusercontent.com/79752672/227696516-d802217b-aefd-49da-b233-944ac750be2d.png)

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

add icon
hide landscape icon
hide parcel
go beyond the template for contrast and legibility

# How to deploy this map?
The client can easily deploy the map style by downloading the json file here: https://github.com/xxxidragons/Zhou_portfolio/blob/bd80a5d27252d9e681681b0f692ddd78a4f80461/CCDC_mapstyle.json 


See more details at: https://developers.google.com/maps/documentation/cloud-customization/map-styles#create-new-style 

Create a page that includes the color palette you used, a screenshot of your stylized map, and a summary of your design decisions.  
You should include an outline of your process from beginning to end, which you'll use to help communicate the steps you took to the organization later.  
Make sure to check your map at various zoom extents to make sure that the maps are usable and legible, especially at the extents most likely to be used by 
the site's visitors.   Changing basemap colors can lead to unanticipated conflicts in layers, so make sure to address any issues you run into as best you ca
n before saving your style.  
