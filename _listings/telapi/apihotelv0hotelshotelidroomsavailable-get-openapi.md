---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Request available rooms using a given criteria.
  version: v0
  description: Request available rooms using a given criteria..
host: api.hetras-certification.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels/{hotelId}/rateplans:
    get:
      summary: Get a list of rateplans for the specified hotel id matching the filter
        criteria.
      description: "With this call you can find rateplans for a hotel by different
        filters. By default and without any filter criteria\r\n            defined
        it will return you all active rateplans."
      operationId: RatePlans_GetRateplans
      x-api-path-slug: apihotelv0hotelshotelidrateplans-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: baseRateplan
        description: Return all rateplans having the specified rateplan as base rateplan
      - in: query
        name: channelCode
        description: Return all rateplans sold through the specified channel
      - in: query
        name: channelGroup
        description: Return all rateplans that are sold through at least one channel
          out of the specified channel group
      - in: query
        name: commissionable
        description: Return all rateplans having commisionable status
      - in: query
        name: group
        description: Return all rateplans belonging to the specified rateplan group
      - in: path
        name: hotelId
        description: The hotel id you are trying to find rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: marketCodes
        description: Return all rateplans having one of the specified values as a
          market code
      - in: query
        name: roomTypes
        description: Return all rateplans by which at least one of the specified room
          types are sold
      - in: query
        name: sellingStatus
        description: Specify which rateplans to return
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: top
        description: Amount of items to select
      responses:
        200:
          description: OK
      tags:
      - Rateplansthe
      - Specified
      - Hotel
      - Id
      - Matching
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rateplans/$count:
    get:
      summary: Get the count of all rateplans in the hotel matching the given filter
        criteria.
      description: Get the count of all rateplans in the hotel matching the given
        filter criteria..
      operationId: RatePlans_GetRateplansCount
      x-api-path-slug: apihotelv0hotelshotelidrateplanscount-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: baseRateplan
        description: Return all rateplans having the specified rateplan as base rateplan
      - in: query
        name: channelCode
        description: Return all rateplans sold through the specified channel
      - in: query
        name: channelGroup
        description: Return all rateplans that are sold through at least one channel
          out of the specified channel group
      - in: query
        name: commissionable
        description: Return all rateplans having commisionable status
      - in: query
        name: group
        description: Return all rateplans belonging to the specified rateplan group
      - in: path
        name: hotelId
        description: The hotel you are counting the rateplans for
      - in: query
        name: includedServices
        description: Return all rateplans having at least one of the specified services
          included
      - in: query
        name: marketCodes
        description: Return all rateplans having one of the specified values as a
          market code
      - in: query
        name: roomTypes
        description: Return all rateplans by which at least one of the specified room
          types are sold
      - in: query
        name: sellingStatus
        description: Specify which rateplans to return
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rateplans
      - In
      - Hotel
      - Matching
      - Given
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rooms:
    get:
      summary: Get a list of rooms using the provided filtering and pagination criteria.
      description: "Find all rooms for the hotel that match the specified filter criteria.
        The filtering will be done based on the current state of\r\n            the
        rooms."
      operationId: Rooms_GetRooms
      x-api-path-slug: apihotelv0hotelshotelidrooms-get
      parameters:
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: conditions
        description: Return results only for rooms that have the given room condition
          status
      - in: path
        name: hotelId
        description: The hotel you are trying to find rooms for
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: maintenances
        description: Return results only for rooms that have the given maintenance
          status
      - in: query
        name: occupancy
        description: Return results only for rooms that have the given frontdesk ocuppancy
          status
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: top
        description: Amount of items to select
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Rooms
      - Using
      - Provided
      - Filtering
      - Pagination
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rooms/$count:
    get:
      summary: Get the count of all rooms in the hotel matching the given filter criteria.
      description: Get the count of all rooms in the hotel matching the given filter
        criteria..
      operationId: Rooms_GetRoomsCount
      x-api-path-slug: apihotelv0hotelshotelidroomscount-get
      parameters:
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: conditions
        description: Return results only for rooms that have the given room condition
          status
      - in: path
        name: hotelId
        description: The hotel you are counting the rooms for
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: maintenances
        description: Return results only for rooms that have the given maintenance
          status
      - in: query
        name: occupancy
        description: Return results only for rooms that have the given frontdesk ocuppancy
          status
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - ""
      - Rooms
      - In
      - Hotel
      - Matching
      - Given
      - Filter
      - Criteria
  /api/hotel/v0/hotels/{hotelId}/rooms/available:
    get:
      summary: Request available rooms using a given criteria.
      description: Request available rooms using a given criteria..
      operationId: Rooms_GetAvailableRooms
      x-api-path-slug: apihotelv0hotelshotelidroomsavailable-get
      parameters:
      - in: query
        name: adults
        description: Specifies number of adults the returned rooms will have to be
          able to house
      - in: query
        name: amenities
        description: Return result only for rooms having all of the given amenities
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: query
        name: from
        description: Rooms returned will not be assigned to a reservation or be under
          maintenance between this date            and the specified to date
      - in: path
        name: hotelId
        description: The hotel you are looking for available rooms
      - in: query
        name: includeOutOfService
        description: Should rooms that are set OutOfService in the defined time period
          be returned as available
      - in: query
        name: inlinecount
        description: Return total number of items for a given filter criteria
      - in: query
        name: locations
        description: Return result only for rooms having at least one of the specified
          locations
      - in: query
        name: roomTypes
        description: Return result only for rooms for the given room types
      - in: query
        name: skip
        description: Amount of items to skip
      - in: query
        name: to
        description: Rooms returned will not be assigned to a reservation or be under
          maintenance between the specified            from date and this date
      - in: query
        name: top
        description: Amount of items to select
      - in: query
        name: views
        description: Return result only for rooms having at least one of the specified
          views
      responses:
        200:
          description: OK
      tags:
      - Request
      - Available
      - Rooms
      - Using
      - Given
      - Criteria
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---