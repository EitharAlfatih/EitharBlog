---
layout: post
title:  "Integrating razorpay into your webapp"
date:   2019-03-23 21:03:36 +0530
categories: Javascript NodeJS
---
To solve the conflict issue in github, follow these steps:  
1-Under your repository name, click  Pull requests.  
2-In the "Pull Requests" list, click the pull request with a merge conflict that you'd like to resolve.
3-Near the bottom of your pull request, click Resolve conflicts.   
4-Decide if you want to keep only your branch's changes, keep only the other branch's changes, or make a brand new change, which may incorporate changes from both branches. Delete the conflict markers <<<<<<<, =======, >>>>>>> and make the changes you want in the final merge.  
5-If you have more than one merge conflict in your file, scroll down to the next set of conflict markers and repeat steps four and five to resolve your merge conflict.    
6-Once you've resolved all the conflicts in the file, click Mark as resolved.  
7-To merge your pull request, click Merge pull request. For more information about other pull request merge options, see "Merging a pull request."

```javascript
const Razorpay = require('razorpay');

let rzp = Razorpay({
	key_id: 'KEY_ID',
	secret: 'name'
});

// capture request
rzp.capture(payment_id, cost)
	.then(function (data) {
		return 2;
	})
```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
