# This repository is used to add [stories](https://blueearthdata.org/stories) to the [BlueEarth Data Platform](https://blueearthdata.org/)

### Instructions:
1. Write and publish a story on an online platform, e.g. https://storymaps.arcgis.com/stories.
2. Create an icon with dimensions `300x280` pixels for the story and give it a human-readable name.
3. Clone / Fetch origin from https://github.com/openearth/bed-stories.
4. Copy the icon you created to the folder `bed-stories/images/`.
5. Open `stories.json` in your preferred text editor.
6. Add a new entry at the top of the `stories.json` file:
```
    {
    "id": "<insert id>",
    "theme": "<insert theme>", # see below available themes
    "stories": [
      {
        "ID": "<insert aplha-numeric-id>",
        "title": "<insert title for story>",
        "URL": "<insert URL to story published on an online platform>",
        "icon": "https://raw.githubusercontent.com/openearth/bed-stories/main/images/<insert filename of icon>"
      }
    ]
    },
```
7. Commit to main and push to origin.
8. Check that everything is as expected in https://blueearthdata.org/stories

**The following themes are availble**
* Flooding
* Coastal Management
* Offshore
* Water availability
* Water quality
* North Sea
* Coastal flood risk
* Small island states

### Known issues
- Stories page doesn't scroll.
- Changes may take a while to reflect due to caching - clear cache if necessary.
