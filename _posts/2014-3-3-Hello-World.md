---
layout: post
title: You're up and running!
---

To recode libc's `printf`.  
  
At 42, students are not allowed to use library functions. We can only submit wholly self-written functions (no `strlen`, `strdup`, `bzero` etc.).
ft_printf must be formatted in the same manor as libc's `printf`. For example:
```c
ft_printf("%s is a %d student\n", "Sietse", 42);
printf("%s is a %d student\n", "Sietse", 42);
```
Should give back:
```console
Sietse is a 42 student
Sietse is a 42 student
```

![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.