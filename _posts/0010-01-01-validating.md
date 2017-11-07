---
layout: slide
title: "Validating"
---

<section markdown="1">
{% highlight sh %}
∫ aws/bastion (master)⮞ terraform validate
{% endhighlight %}

{% highlight sh %}
Error validating: 3 error(s) occurred:

* Variable 'security_groups': duplicate found. Variable names must be unique.
* output 'role': unknown resource 'aws_iam_role.bast' referenced in variable aws_iam_role.bast.name
* resource 'aws_instance.bast' config: unknown resource 'aws_iam_instance_profile.bast' referenced in variable aws_iam_instance_profile.bast.name
{% endhighlight %}

