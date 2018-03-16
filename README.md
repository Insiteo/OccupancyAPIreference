
This page describes the format of Insiteo's API providing real-time room availability information.

## Authentication

Endpoints require a valid APIKey to be included in the request header.
`APIKey: yourAPIKey`

### Endpoints

Each endpoint provides real-time status of Rooms for the requested account:

* [Show all rooms' occupancy information](RoomOccupancy.md) : `GET /RoomOccupancy/`
* [Show detailed information about busy rooms](RoomStatus.md) : `GET /RoomStatus/`
* [Show detailed information about busy rooms for a given Site](RoomStatus.md) : `GET /RoomsStatusForSite/{SiteID}/`
