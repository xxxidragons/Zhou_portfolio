# Phase 1: Bid development

https://www.chinatowncdc.org/

# Generate a custom palette
I use Canva's color palette generator to generate my color palatte based on one of the pics from CCDC website.
![colorpalatte](https://user-images.githubusercontent.com/79752672/227689759-16d91319-3678-4712-b0a4-5d17f3b90512.png)
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
# Build custom map using the Google Map Styling Wizard

![scale0](https://user-images.githubusercontent.com/79752672/227696114-259588ec-0d23-441d-9a37-1a1c5575e7a2.png)
![scale1](https://user-images.githubusercontent.com/79752672/227696117-15eb7298-c097-44ea-baad-1926fdef80e7.png)
![scale2](https://user-images.githubusercontent.com/79752672/227696115-906e32e3-eac3-4ed0-9732-d081324db15d.png)
![scale3](https://user-images.githubusercontent.com/79752672/227696516-d802217b-aefd-49da-b233-944ac750be2d.png)
add icon
hide landscape icon
hide parcel
go beyond the template for contrast and legibility

Here is the link of downloadable JSON code:
https://github.com/xxxidragons/Zhou_portfolio/blob/bd80a5d27252d9e681681b0f692ddd78a4f80461/CCDC_mapstyle.json 

The development team has requested the ability to easily embed the redesigned basemap into the existing website.  
To help with this, the consultant will create simple instructions documenting the provided materials and how to effectively use them. 

https://developers.google.com/maps/documentation/cloud-customization/map-styles#create-new-style 

Create a page that includes the color palette you used, a screenshot of your stylized map, and a summary of your design decisions.  
You should include an outline of your process from beginning to end, which you'll use to help communicate the steps you took to the organization later.  
Make sure to check your map at various zoom extents to make sure that the maps are usable and legible, especially at the extents most likely to be used by 
the site's visitors.   Changing basemap colors can lead to unanticipated conflicts in layers, so make sure to address any issues you run into as best you ca
n before saving your style.  
