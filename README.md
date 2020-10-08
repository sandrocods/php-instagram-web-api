# Instagram Web API Client ❤️️📷
A PHP 7.2+ Function to read and process Instagram Client.
This library requires [Curl](https://www.php.net/manual/en/book.curl "Curl") ,extensions installed.

## How to usage
### Authenticate Instagram Account
```php
include 'Instagram_Web_API/InstagramFunc.php';
$login = login('Username','Password',Cookie());
```
U can save Cookie with
```php
Savecookie('Username',$login);
```
### Example login using cookie
```php
include 'Instagram_Web_API/InstagramFunc.php';
$login_cookie = Logincookie('mayanasution4');
$Geteditprofile = Geteditprofile($login_cookie);
print_r($Geteditprofile);
```
## Feature
| Feature  | Available  |
| ------------ | ------------ |
|  [GetCookie](#GetCookie) |  ✔️ |
|  [Login](#Login) |  ✔️ |
|  [LoginCookie](#LoginCookie) |  ✔️ |
|  [InfoAccount](#InfoAccount) |  ✔️ |
|  [Follow](#Follow) |  ✔️ |
|  [Unfollow](#Unfollow) |  ✔️ |
|  [Like](#Like) |  ✔️ |
|  [Unlike](#Unlike) |  ✔️ |
|  [Comment](#Comment) |  ✔️ |
|  [Uncomment](#Uncomment) |  ✔️ |
|  [GetComment](#GetComment) |  ✔️ |
|  [LikeComment](#LikeComment) |  ✔️ |
|  [Savemedia](#Savemedia) |  ✔️ |
|  [Getactivity](#Getactivity) |  ✔️ |
|  [Gethome](#Gethome) |  ✔️ |
|  [Geteditprofile](#Geteditprofile) |  ✔️ |
|  [Editprofile](#Editprofile) |  ✔️ |
|  [Changepassword](#Changepassword) |  ✔️ |
|  [fetch_inbox](#fetch_inbox) |  ✔️ |
|  [delete_inbox](#delete_inbox) |  ✔️ |
|  [Changeprofile](#Changeprofile) |  ✔️ |
|  [Removeprofilepicture](#Removeprofilepicture) |  ✔️ |
|  [Savecookie](#Savecookie) |  ✔️ |


## Example

### GetCookie
```php
$cookie = Cookie();
```
> return Csrf , Mid , Ig_did

### Login
```php
$login = login('Username','Password',Cookie());
```
### LoginCookie
```php
$login_cookie = Logincookie('Username');
```

### InfoAccount
```php
$InfoAccount = InfoAccount($username, $login_cookie)
```

### Follow
```php
$Follow = Follow($user_id, $login_cookie);
```

### Unfollow
```php
$Unfollow = Unfollow($user_id, $login_cookie);
```

### Like
```php
$Like = Like($media_id, $cookie);
```

### Unlike
```php
$Unlike = Unlike($media_id, $cookie);
```

### Comment
```php
$Comment = Comment($media_id, $text, $cookie);
```
### Uncomment
```php
$Uncomment = Uncomment($media_id, $comment_id, $cookie)
```
### Unlike
```php
$Unlike = Unlike($media_id, $cookie)
```
### Unlike
```php
$Unlike = Unlike($media_id, $cookie)
```
### Getcomment
```php
$Getcomment = Getcomment($shortcode, $cookie);
```
### Likecomment
```php
$Likecomment = Likecomment($comment_id, $cookie);
```
### Savemedia
```php
$savemedia = Savemedia($media_id, $cookie);
```
### Getactivity
```php
$getactivity = Getactivity($cookie);
```
### Gethome
```php
$timeline = Gethome($cookie, $End_cursor = null);
```
### Geteditprofile
```php
$geteditprofile = Geteditprofile($cookie);
```
### Editprofile
```php
$Editprofile = Editprofile($cookie, $first_name, $email, $username, $phone_number, $biography);
```
### Changepassword
```php
$changepassword = Changepassword($cookie, $old_password, $new_password);
```
### fetch_inbox
```php
$fetch_inbox = fetch_inbox($cursor = null, $cookie);
```
### delete_inbox
```php
$delete_inbox = delete_inbox($thread_id, $cookie);
```
### Changeprofile
```php
$Changeprofile = Changeprofile($cookie, $path_image);
```
### Removeprofilepicture
```php
$Removeprofilepicture = Removeprofilepicture($cookie);
```
### Savecookie
```php
$Savecookie = Savecookie($username , $cookie);
```
