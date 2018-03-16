# Show Accessible Accounts

Show all Accounts the active User can access and with what permission level.
Includes their own Account if they have one.

**URL** : `/RoomOccupancy/`

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
    "SiteID":332,
    "RoomStatusList":[
      {
        "CommonKey":"CommonKey-1",
        "IsBusy":false,
        "NbPhysicalUsers":0,
        "RoomName":"Room1"
      },
      {
        "CommonKey":"CommonKey-2",
        "IsBusy":true,
        "NbPhysicalUsers":3,
        "RoomName":"Room2"
      },
      {
          "CommonKey":"CommonKey-3",
          "IsBusy":true,
          "NbPhysicalUsers":0,
          "RoomName":"Room3"
      }
    ]
  },
  {
    "SiteID":337,
    "RoomStatusList":[
      {
        "CommonKey":"POI01",
        "IsBusy":false,
        "NbPhysicalUsers":0,
        "RoomName":"POI01"
      },
      {
        "CommonKey":"POI02",
        "IsBusy":true,
        "NbPhysicalUsers":0,
        "RoomName":"POI02"
      }
    ]
  }
]
```
