# Research
Every student selects a subject, relevant directly to one of the projects, or to one of the subjects within this course. 
#### [More information](https://fhict.instructure.com/courses/12992/pages/research-reports-bachelor-students-only?module_item_id=911565)

#### questions
What is the best way to implement an interactive map in my application?
- What is the implementation in my application?

My application is a website for divers to get an overview of diving locations and fish. Have an interactive world map that shows diving locations that are clickable. When clicked show information about dive and fish at that location. Have a search function for both dives and fish. Dive listing shows information about that dive and which fish a diver would be able to see when taking that dive. Fish listing shows information about that fish and which diving locations a diver would be able to see that fish at.
- What can be used to implement an interactive map in my application?

[Leaflet](https://leafletjs.com/) /
[Nominatim](https://nominatim.openstreetmap.org/ui/search.html) /
[OpenStreetMap](https://www.openstreetmap.org/#map=7/52.154/5.295) /
[AmplifyGeo](https://aws.amazon.com/blogs/mobile/add-interactive-maps-in-react-using-amplify-geo/)

React Simple Maps, Google Map React, Deck.gl, React Leaflet, Pigeon Maps

- What are the pros and cons of these methods in my application?
##### React Simple Maps
Pros
- This library renders the map as an SVG, which makes it very easy to handle with HTML.
- Extensible with other React components.
- A lightweight library.


Cons
- Performance issues when working with extensive map data.
- Smaller developer community.

##### Google Map React
Pros
- Supports custom map markers with hover effects.
- Uses the content-rich Google Map API to fetch map data.
- Isomorphic rendering — map rendering support on both client and server-side.
- If the API is not responding, Google Map React can render basic map components locally in the browser.

Cons
- Requires setting up a Google developer account and API key.
- For production and extensive use, you need to purchase Google Map Service.

##### Deck.gl
Pros
- Highly extensible and customizable library.
- Performant rendering and updating of large data sets.
- Interactive event handling such as picking, highlighting, and filtering.
- In-built support for different layer types such as icons, polygons, texts; and different views such as first-person, orthographic.
- Supports integrations with major base map providers, including Mapbox, Google Maps, and more.

Cons
- Heavy memory demand from clients’ machines to render a map.
- Less browser compatibility and less cross-platform support.

##### React Leaflet
Pros
- Simple library with fine-tuned basic features.
- Cross-browser and platform support.
- Layer customizations.
- Mobile responsiveness.

Cons
- Server-side rendering is not supported.
- Direct DOM calls are made during the loading phase, which might be a bummer for handling extensive map data.

##### Pigeon Maps
Pros
- Lightweight and fast map rendering.
- Custom map tile provider support.
- Mobile optimized map controls.

Cons
- Less extensibility with other components.
- Advanced map customizations are not possible.

#### methods
#### execution
#### results
For my application the Google Map React API wil work the best, it has the customisation that I am looking for and great documentaion.  
