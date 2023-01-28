# api
Our API that is accessable for our users to use.

You need to get your API key from our site, this is accessable to users that have an account with us at [Planet Xylox](https://planetxylox.com), this is for those that want some information which we're open to make public!

### `api/users?key=[API_KEY]` [GET method]

Returns:

```
{
"total_users": INT,
"staff_users": INT,
"verified_users": INT,
"unverified_users": INT,
"banned_users": INT,
"blacklisted_users": INT
}
```

### `api/global?key=[API_KEY]` [GET method]

Returns:

```
{
"total_characters": INT,
"total_dressup_characters": INT,
"total_dressup_items": INT,
"total_guestbook_msgs": INT,
"total_quiz_questions": INT,
"total_faq_questions": INT
}
```

### `api/user=[username]&key=[API_KEY]` [GET method]

Returns:

```
{
"username": STRING,
"reg_date": INT,
"bio": STRING,
"favorite_char": STRING,
"current_char": STRING,
"country": STRING
}
```

### `api/userDressup?user=[username]&char_id=[character ID]&key=[API_KEY]` [GET method]

Returns:

```
{
"username": STRING.
"character": STRING,
"dressup" ARRAY: [
  "name": STRING,
  "description": STRING,
  "src": BASE64 STRING
]
}
```




