# flickr-to-smugmug

Tool to import my flickr to smugmug.

# Via flickr export and SmugMug API

1. Export all your data (including JSON)
2. Unzip it all

## JSON Files

Sample list:

```
account_profile.json
account_testimonials.json
albums.json
apps_comments_part001.json
contacts_part001.json
faves_part001.json
followers_part001.json
galleries.json
galleries_comments_part001.json
group_discussions.json
groups.json
photo_*.json
photos_comments_part001.json
received_flickrmail_part001.json
sent_flickrmail_part001.json
sets_comments_part001.json
```

### albums.json

```json
{
  "albums": [
    {
      "photo_count": "[int]",
      "id": "[int]",
      "url": "https://www.flickr.com/photos/[string]/albums/[int]",
      "title": "Title goes here",
      "description": "Description goes here",
      "view_count": "0",
      "created": "[int timestamp]",
      "last_updated": "[int timestamp]",
      "cover_photo": "https://www.flickr.com/photos/[string]/[int]",
      "photos": [
        "[int photo id]",
```

### photo_[int].json

```json
{
  "id": "[int photo id]",
  "name": "",
  "description": "",
  "count_views": "0",
  "count_faves": "0",
  "count_comments": "0",
  "date_taken": "YYYY-MM-DD hh:mm:ss",
  "count_tags": "0",
  "count_notes": "0",
  "rotation": 0,
  "date_imported": "YYYY-MM-DD hh:mm:ss",
  "photopage": "https://www.flickr.com/photos/[string]/[int]/",
  "original": "https://live.staticflickr.com/[int]/[id].jpg",
  "license": "All Rights Reserved",
  "geo": {
    "latitude": "[int]",
    "longitude": "[int]",
    "accuracy": "[int]"
  },
  "groups": [],
  "albums": [],
  "tags": [],
  "people": [],
  "notes": [],
  "privacy": "private",
  "comment_permissions": "any flickr member",
  "tagging_permissions": "people you follow",
  "safety": "safe",
  "comments": []
}
```
