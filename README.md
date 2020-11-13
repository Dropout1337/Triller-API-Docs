# Triller API Documentation
[Triller](https://triller.co/) Is A Soical Media/Video Sharing App Like TikTok
So I Decided To Make A Little Documentation For It.

# API Endpoints
## Play/View Video
```
Post: https://social.triller.co/v1.5/api/videos/play
Json: {
            "auth_token": "Triller_Auth_Token_Here",
            "sound_active": true,
            "video_id": Video_ID
      }
```

## Create/Make Account
```
Post: https://social.triller.co/v1.5/user/create
Json: {
            "app_version": "18.0",
            "email_address": "Email_Here",
            "username": "Username_Here",
            "password": "Password_Here",
            "push_token": "",
            "platform": "iOS"
      }
```

## Login/Check Account
```
Post: https://social.triller.co/v1.5/user/auth
Json: {
            "password": "Password_Here",
            "app_version": "18.0 (1827)",
            "push_token": "",
            "platform": "iOS",
            "api_version": "v1.5",
            "username": "Username/Email_Here",
            "language_code": "en-NZ"
      }
```

## Like/Heart Video
```
Post: https://social.triller.co/v1.5/api/videos/like
Json: {
            "video_id": Video_ID,
            'auth_token': "Auth_Token"
      }
```

## Comment On Video
```
Post: https://social.triller.co/v1.5/api/videos/VIDEO_ID/comments/
Json: {
            "body": "Comment_Here",
            'auth_token': "Auth_Token"
      }
```

## Report User
```
Post: https://social.triller.co/v1.5/api/users/flag
Json: {
            'flagged_user_id': User_ID,
            'auth_token': "Auth_Token",
            'reason': "Reason_Here"
      }
```

## Report Video
```
Post: https://social.triller.co/v1.5/api/video/flag
Json: {
            'flagged_video_id': Video_ID,
            'auth_token': "Auth_Token",
            'reason': "Reason_Here"
      }
```

## Like Video Comment
```
Post: https://social.triller.co/v1.5/api/comments/like
Json: {
            "app_version": "18.0 (1827)",
            "platform": "iOS",
            "api_version": "v1.5",
            "language_code": "en-NZ",
            "auth_token": "Auth_Token",
            "comment_id": "Comment_ID"
      }
```

## Follow User
```
Post: https://social.triller.co/v1.5/api/users/follow
Json: {
            'followed_ids': User_ID,
            'auth_token': "Auth_Token",
      }
```

## Unfollow User
```
Post: https://social.triller.co/v1.5/api/users/follow/delete
Json: {
            'followed_ids': User_ID,
            'auth_token': "Auth_Token",
      }
```

# Thanks For Checking My Documentation Out
Please Make An Issue If You Want Me To Add Somthing <3
