

First, you need to create a `Users` object from the `Users` class in the `tiktok_users` module:

```python
from khang import Users

getTiktokUser = Users()
```

Then, you can call the `details` method of this object and pass the TikTok username as an argument:

```python
username = "@USERNAME"  # Replace USERNAME with the TikTok username you want to query
result = getTiktokUser.details(username)
print(result)
```

And here's a sample JSON response and explanation of each parameter:

```json
{
  "code": 200,
  "user": {
    "id": "6728368430175159297",
    "username": "phuong lien 🍳",
    "profileName": "phuoglienzxx_",
    "avatar": "https://p16-sign-sg.tiktokcdn.com/aweme/720x720/tos-alisg-avt-0068/c46532ef63837ef61c4a2079ed4beb50.jpeg?lk3s=a5d48078&nonce=68232&refresh_token=ed4fce6885daf1b16447883e1b86ba3b&x-expires=1716120000&x-signature=%2FNcEGijZyjGGe5XnyKjwdwz9iFg%3D&shp=a5d48078&shcp=81f88b70",
    "description": "dang di tam",
    "region": "VN",
    "verified": false
  },
  "stats": {
    "following": 4,
    "follower": 1211,
    "video": 2,
    "like": 3161
  }
}
```

- `code`: The status code of the response (200 indicates success).
- `user`: Information about the TikTok user.
  - `id`: User ID.
  - `username`: TikTok username.
  - `profileName`: Unique profile name.
  - `avatar`: URL of the user's avatar.
  - `description`: User's profile description.
  - `region`: User's region.
  - `verified`: Boolean indicating if the user is verified.
- `stats`: Statistics about the user.
  - `following`: Number of users the user is following.
  - `follower`: Number of followers the user has.
  - `video`: Number of videos posted by the user.
  - `like`: Number of likes received by the user.

