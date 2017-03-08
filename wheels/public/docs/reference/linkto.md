```coldfusion
#linkTo(text="Log Out", controller="account", action="logout")#
-> <a href="/account/logout">Log Out</a>

// If you're already in the `account` controller, CFWheels will assume that's where you want the link to point 
#linkTo(text="Log Out", action="logout")#
-> <a href="/account/logout">Log Out</a>

#linkTo(text="View Post", controller="blog", action="post", key=99)#
-> <a href="/blog/post/99">View Post</a>

#linkTo(text="View Settings", action="settings", params="show=all&amp;sort=asc")#
-> <a href="/account/settings?show=all&amp;amp;sort=asc">View Settings</a>

// Given that a `userProfile` route has been configured in `config/routes.cfm` 
#linkTo(text="Joe's Profile", route="userProfile", userName="joe")#
-> <a href="/user/joe">Joe's Profile</a>

// Link to an external website 
#linkTo(text="ColdFusion Framework", href="http://cfwheels.org/")#
-> <a href="http://cfwheels.org/">ColdFusion Framework</a>

// Give the link `class` and `id` attributes 
#linkTo(text="Delete Post", action="delete", key=99, class="delete", id="delete-99")#
-> <a class="delete" href="/blog/delete/99" id="delete-99">Delete Post</a>
```