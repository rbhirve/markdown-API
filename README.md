# SumHR REST API Docs:

These examples were taken from projects mainly using 
JSON responses are often similar to the way in which DRF makes responses.

## Open Endpoints

Open endpoints require no Authentication.

* [User Login](login.md) : `POST /api/sumhr/login/`

## Endpoints that require Authentication

Closed endpoints require a valid Token to be included in the header of the
request. A Token can be acquired from the Login view above.

### Attendance Cycle API

Endpoints for viewing and manipulating the Accounts that the Authenticated User has permissions to access.

* [Create Attendance Cycle](attendance/cycle/post.md) : `POST /attendance/settings/createattendancecycle/`
* [Edit Attendance Cycle](attendance/cycle/get.md) : `GET /attendance/settings/editattendancecycle/8/`
* [Delete Attendance Cycle](attendance/cycle/delete.md) : `DELETE /attendance/settings/deleteattendancecycle/8/`
