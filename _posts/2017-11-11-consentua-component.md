---
layout: post
title: consentua-component
published: false
author: jack_mason
comments: true
---

>A web component for interfacing with Consentua (get and set user consents), built on Polymer2

![consentua-component](https://cl.ly/1N262o3R1l0H/Image%202017-10-27%20at%2012.18.38%20PM.png)

## Usage

{% highlight html %}
<consentua-component key="19fb13ab-d6f2-42dc-a41c-42249450b5b6"
                               device-id="ACoolAndUniqueDeviceID"
                               service-id="1"
                               client-id="2"
                               user-identifier="demo@test.com">
                               </consentua-component>
{% endhighlight %}
* *key*, *service-id*, *client-id* - Will be provided to you when you sign up with Consentua
* *device-id* - recommend using [fingerprintjs2](http://valve.github.io/fingerprintjs2/)
* *user-identifier* - A user identifier, we recommend an email address

You can find it [here](https://www.webcomponents.org/element/mrsideshowjack/consentua-component)

Feel free to contribute to it [here](https://github.com/mrsideshowjack/consentua-component)
