```php
$eval[$replaceText[$message;$$c[]eval[;$$c[]var[_ei\;$$c[]sum[0$$c[]var[_ei\]\;1\]\]$$c[]var[_e$$c[]var[_ei\]\;]]
$eval[$var[_e1]]$eval[$var[_e2]]$eval[$var[_e3]]$eval[$var[_e4]]$eval[$var[_e5]]$eval[$var[_e6]]$eval[$var[_e7]]
```
This works by evaluating the code in a separate eval. If you use this code, you can only use eval in eval 7 times, and the other ones will just be ignored. You can add more to the end (like `$eval[$var[_e8]]`) to increase that limit.

# Actual usage example
```php
!eval
$textSplit[$userRoles[$authorID];$url[decode;%0A]]
$eval[$$c[]roleGrant[$$c[]authorID\;-$$c[]roleID[$joinSplitText[\]\;-$$c[]roleID[]\]\]]
```
This should in theory remove all of the roles of the person that uses it.
