# RetractableToolbar

<span class="badge-paypal"><a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&amp;hosted_button_id=LY7EX8WMWPWV6" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-yellow.svg" alt="PayPal donate button" /></a></span>
[![Twitter](https://img.shields.io/badge/Twitter-@LacorteMichele-blue.svg?style=flat)](https://twitter.com/LacorteMichele)

[![API](https://img.shields.io/badge/API-21%2B-blue.svg?style=flat)](https://android-arsenal.com/api?level=21)

[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-RetractableToolbar-brightgreen.svg?style=flat)](http://android-arsenal.com/details/1/2844)

[![alt tag](http://www.android-gems.com/badge/michelelacorte/RetractableToolbar.svg)](http://www.android-gems.com/lib/michelelacorte/RetractableToolbar?lib_id=709)

![alt tag](http://i.giphy.com/3oEduTiPtJGG9Q23Xq.gif)

Retractable Toolbar it is a utility to give the effect Retractable your toolbar!!

##USAGE

Retractable Toolbar is pushed to JCenter, so you just need to add the following dependency to your `build.gradle`.
```
compile 'it.michelelacorte.retractabletoolbar:library:1.0.0'
```

In alternative you can use AAR repository with:

```
allprojects {
    repositories {
        maven { url "https://dl.bintray.com/michelelacorte/maven/" }
        jcenter()
        mavenCentral()

    }
}
```

And add this dependecies

```
compile 'it.michelelacorte.retractabletoolbar:library:1.0.0@aar'
```

In your `MainActivity.java`

```
RetractableToolbarUtil.ShowHideToolbarOnScrollingListener showHideToolbarListener;
recyclerView.addOnScrollListener(showHideToolbarListener = new RetractableToolbarUtil.ShowHideToolbarOnScrollingListener(toolbar));

if (savedInstanceState != null) {
            showHideToolbarListener.onRestoreInstanceState((RetractableToolbarUtil.ShowHideToolbarOnScrollingListener.State) savedInstanceState
                    .getParcelable(RetractableToolbarUtil.ShowHideToolbarOnScrollingListener.SHOW_HIDE_TOOLBAR_LISTENER_STATE));
}
```

##SYSTEM REQUIREMENT

Android API 21+

##CHANGELOG

**v1.0.0**
- Support API 21+
- Support `RecyclerView` list

##CREDITS

Author: Michele Lacorte (micky1995g@gmail.com)

##LICENSE

```
Copyright 2015 Michele Lacorte

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
