# cs1660-finalproject
A garbage static webapp that demonstrates Miracle Sort.

# LIVE NOW AT: http://cs1660.dev

## What is Miracle sort?
Simple:

```
list = [...]

while list is not sorted:
    pass

return "It's sorted!"
```


If some list is not sorted, keep checking until by some miracle the list is actually sorted!

See [this](https://pages.cs.wisc.edu/~okushi/) for more.

## How does this work

I am faithfully recreating this algorithm with hacked-together javascript intervals and array ops.

On initial page load, we Fisher-Yates shuffle a 100-element array. Every second, we check if this array is sorted and update the user if this has happened. Our array is rendered as a bar chart for visulalization purposes. User will see a running total of time ~~wasted~~ spent waiting for our miracle.

## Frontend dev

UI design [is my passion](https://i.kym-cdn.com/photos/images/original/001/018/866/e44.png) so I just modified the standard demo Bootstrap template. Fight me. Bar chart generation is some basic CSS div-ing.

## Backend dev

This is a very-simple static site hosted using GCP's storage buckets. I followed [Google's tutorial](https://cloud.google.com/storage/docs/hosting-static-website-http). Building [a load balancer just to use https](https://cloud.google.com/storage/docs/hosting-static-website) feels like a GCP problem, not mine. I didn't burn my credits on forgotten VMs so I bought the domain name via Cloud Domain. I also followed the tutorial and uploaded my html through console (I am still traumatized by the IAM assignment and did not attempt Github Actions or the like).

## What did I learn

I don't like frontend web app development.

## Final thoughts

Thanks for a great semester!