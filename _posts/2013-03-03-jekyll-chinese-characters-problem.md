---
layout: post
title: "Jekyll Server中文问题"
description: ""
category: Tips
tags: [Jekyll, Ruby, Tips]
---
{% include JB/setup %}

用Jekyll已经发过几篇文章了，中英文都有，可是最近发现在搭建本地Server老是有问题，新的文章显示不出来。在Console上面能看到一段Warning.

>Could not determine content-length of response body. Set content-length of the response or set Response#chunked = true

我想这一定跟字符编码有关，果然定位到是中文文章照成的。于是在网上搜索解决办法，原来跟Ruby有关。需要修改`ruby/gems/1.9.1/jekyll-0.11.2/lib/jekyll/convertible.rb`

	Line 27
	self.content = File.read(File.join(base, name), :encoding => "utf-8")

