Sina Weibo Follow and Share Buttons for Octopress
====

Description:
----
This plugin adds [Sina Weibo](http://weibo.com) follow button to the Octopress sidebar.
It also adds share button at the bottom of the blog entry.

Files:
----

To add follow button:
Place `source/_includes/custom/asides/weibo.html` in `source/_includes/custom/asides/`.

To add share button:
Place `source/_includes/custom/post/sharing.html` in `source/_includes/custom/post/`.

Configuration:
----

To add follow button:

Add `custom/asides/weibo.html` to `default_asides:` in your `_config.yml`.

Add the Weibo sidebar configuration options to your `_config.yml` at the bottom of "3rd Party
Settings". You'll need your Weibo user id, which is different from your username. Go to your weibo.com
profile page.  You should see a url like this: http://www.weibo.com/u/2091903003, right below your user name.
The last part of the url (long digits after http://www.weibo.com/u/) is your user ID.

```yaml
# Sina Weibo
weibo_user: 2091903003 #user id (not user name)
```

To add share button, edit _config.yml and add:

```yaml
# Sina Weibo
weibo_user: 2091903003 #user id (not user name)
weibo_share_button: true
```

Run `rake generate` since _config.yml has been changed.

Example
----

See [@zlu](http://www.zlu.me).  Follow button is at the bottom of the right side.  Share button is at the bottom
of every blog entry.

License
----

(The MIT License)

Copyright © 2012 Zhao Lu

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the ‘Software’), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED ‘AS IS’, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.