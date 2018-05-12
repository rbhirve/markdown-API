# Delete Attendance's Cycle

Delete the Cycle of the Authenticated User if they are Owner.

**URL** : `/attendance/settings/deleteattendancecycle/29/`

**URL Parameters** : `pk=[integer]` where `pk` is the ID of the Account in the
database.

**Method** : `DELETE`

**Auth required** : YES

**Data** : `{}`

## Success Response

**Condition** : If the Account exists.

**Code** : `{
    "status": true,
    "message": "Attendance Cycle setting deleted successfully!",
    "data": null
}`

**Content** : `{}`

## Error Responses

**Condition** : If there was no Account available to delete.

**Code** : `404 NOT FOUND`

**Content** : `{}`

### Or

**Condition** : Authorized User is not Owner of Account at URL.

**Code** : `403 FORBIDDEN`

**Content** : `{}`


## Notes

* Will remove memberships for this Account for all Users that had access.
