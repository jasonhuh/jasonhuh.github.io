---
layout: post
title: Launching GeekDojo.io
permalink: /2018/02/16/launching-geekdojo-io
---



### Once upon a time...
Several months ago, I launched an education program ([Bellevue Code School](http://www.bellevuecodeschool.com)) and held an in-person class on a weekly basis. After each class, students were assigned homework. Since they are bright young students who just began to learn programming, they naturally relied on the website's homepage. I originally designed the website using the Hugo platform because I wanted the website to be super fast and durable with the AWS CloudFront and S3 static hosting.

### Launch of GeekDojo.io
As the contents grew, I had to find a way to boost my productivity through a WordPress platform which provides rich set of templates and plugins backed by huge online community. So, I launched a website called [GeekDojo.io](https://geekdojo.io) using WordPress with BlueHost where I hosted other websites. The performance of the WordPress admin site was quite bad that now the bottleneck for my productivity was the WordPress admin site that I have to use to generate contents. If it was a client facing website, sure, I can use caching or CND to boost performance. But if the issue is a performance with a WordPress admin site, the only option is 1) you have to upgrade a web hosting plan or 2) switch a web hosting provider.

### WordPress Hosting in AWS
I chose the 2nd option, and I decided to look elsewhere. I thought about other web hosting providers, but since I am quite familiar with the Amazon AWS products, as an experiment, I launched a WordPress site using AWS ELB and AWS Autoscaling group for scalability/durability, and I used AWS CloudFront for performance. I also optimized the WordPress to host media files in an S3 bucket which is also backed by AWS CloudFront.

{{<figure src="/img/geekdojo.png" title="Screenshot of GeekDojo.io">}}

I was pleasantly surprised with the performance gain I achieved for both the front-end and the admin site. Also, I felt a tighter control of security and backup strategy.

For my personal blog, I am still using [Hugo Server](https://gohugo.io/commands/hugo_server/) with the combination of AWS S3 and CloudFront because I have a tighter control of template rendering and because I like the idea of minimizing waste by avoiding servers to be up and running even when nobody is visiting my blog.

### Summary
On a final thought, if your purpose is to host a simple WordPress website or if you do not have technical background in AWS, I would recommend not to use AWS for hosting a WordPress website unless your main purpose is to simply learn AWS. It is because hosting a WordPress site in AWS is, in general, _significantly_ more expensive compared to using a web hosting provider. But if you are willing to control every aspect of your website and if you need a high performing, fault-tolerant, scalable web solution, Amazon AWS is one of the best solutions out there.

### Resources
For those who are interested in hosting a WordPress site in AWS, here are couple of resources:

* [How to accelerate your WordPress site with Amazon CloudFront](https://aws.amazon.com/blogs/startups/how-to-accelerate-your-wordpress-site-with-amazon-cloudfront/)
* [Launch a WordPress Webiste with Amazon AWS](https://aws.amazon.com/getting-started/tutorials/launch-a-wordpress-website/)
* [SSL Install with AWS ELB and WordPress](https://docs.bitnami.com/aws/how-to/configure-elb-ssl-aws/)
