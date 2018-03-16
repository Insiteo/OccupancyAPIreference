# Show detailed occupancy status for all Busy rooms

**URL** : `/RoomStatus/`

**Method** : `GET`

**Auth required** : YES

**Permissions required** : None

**Data constraints** : `{}`

## Success Responses

**Condition** : User can not see any Sites or Invalid APIKey

**Code** : `200 OK`

**Content** : `{[]}`

### OR

**Condition** : User can see one or more Sites.

**Code** : `200 OK`

**Content** : In this example, information for 2 sites are returned.


```json

[
  {
    "SiteID":337,
    "RoomsList":[
      {
        "CommonKey":"poi-1",
        "RoomName":"NameA",
        "Users":["b1bd1ec7-568a-4d00-a8d3-cc227376f22e","3838aec7-568a-4d00-dede-cc227376f16a"]
      },
      {
      "CommonKey":"poi-2",
      "RoomName":"NameB",
      "Users":["IR Desk Sensor","IR Desk Sensor","IR Room Sensor"]
      }
    ]
  }
]


```
