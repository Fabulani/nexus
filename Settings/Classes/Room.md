---
limit: 20
mapWithTag: true
icon: door-open
tagNames: 
filesPaths: 
bookmarksGroups: 
excludes: 
extends: 
savedViews: 
favoriteView: 
fieldsOrder:
  - lGEvv0
  - AukFwL
  - oU0atp
  - OhoeGW
version: "2.15"
fields:
  - name: inside_of
    type: File
    options: {}
    path: ""
    id: OhoeGW
  - name: floor
    type: Number
    options:
      step: 1
      min: 0
    path: ""
    id: oU0atp
  - name: type
    type: Select
    options:
      sourceType: ValuesListNotePath
      valuesList: {}
      valuesListNotePath: Settings/Fields/room type.md
    path: ""
    id: AukFwL
  - name: area_m2
    type: Number
    options:
      min: 0
    path: ""
    id: lGEvv0
---
Represents rooms inside buildings. Should contain containers or items, and be a part of a building.