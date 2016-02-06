# Performance Testing for Modern Apps
### Dustin Whittle | @dustinwhittle | http://speakerdeck.com/dustinwhittle

## Why does Performance matter?
Performance directly impacts the bottom line
Performance is key to a great user experience

## Apache Bench
Already included in apache
`ab -c 1 -t 10 -k http://example.com` 

## Siege
`siege -c 10 -b -t 10S http://example.com`

## What about when you need more thatn one machine?
Bees with machine guns tool used on ec2 instances (AWS)
`pip install beeswithmachinegus`

## Locust.io
http://github.com/locustio/locust 

`pip installl locustio`

### Many other tools
- Gatling.io
- Wrk
- Vegeta
- Tsung
- ...

In modern web applications more latency comes from the client-side than the server-side

## Tools
- [PageSpeed Insights](http://google.com/pagespeed)
- (http://github.com/pagespeed/ngx_pagespeed)
- `npm install psi` <-- pretty cool CLI 
- http://webpagetest.com
- sitespeed.io

## Things to do

- Automate clien-side perfomance testing with grunt/gulp. 
- Instrument everything = code, DBs, caches, queues, third party services, etc
- Track performance in development and production.

## Best Practices
- Treat perfomance as a feature
- Capacity plan and load test the server-side
- Optimize and performance test the client-side
- Understand your starting point
- Instrument everything
- Monitor perfomance in development and production
- Measure the difference of every change
- Automate performance testing in your build and deployment process
- Understand how failures impact performance

## The protocols are eveolving
- HTTP/2
- 	Yous hosuld unshard, unconcat, and unsprite your assets
-  You should push asstets instead
