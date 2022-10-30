---
name: Remove favorite map

url: https://api.trackmania.com
method: GET
route: /api/user/maps/favorite/remove

audience: n/a

---

The request body is a JSON object containing the map's UID:
```json
{
  "uid": "JlxlB7KbrCfhjAf5ld89ByXR987"
}
```

---

Removes a map from the player's favorite maps.

---

**Remarks**:
- This endpoint requires the `write_favorite` scope.
- The access token has to be provided in the `Authorization` header in the format `Bearer <token>`.

---

**Example request**:
```plain
POST https://api.trackmania.com/api/user/maps/favorite/remove
```
```json
{
  "uid": "JlxlB7KbrCfhjAf5ld89ByXR987"
}
```

**Example response**:
The response will be empty with a `204` response code.