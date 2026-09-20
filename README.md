# Static Website Hosting on AWS (S3 + CloudFront)

Hosted my portfolio website on AWS using a private S3 bucket and CloudFront (HTTPS).

## Services used
- Amazon S3 (private bucket)
- Amazon CloudFront (CDN + HTTPS)

## What I did
- Created an S3 bucket with Block Public Access turned on
- Uploaded website files (HTML, CSS, images)
- Created a CloudFront distribution with private bucket access
- Set the default root object to index.html
- Re-uploaded updated files to S3 after making changes
- Deleted the CloudFront distribution and S3 bucket after testing to avoid costs

## Live site
Deployed on AWS S3 + CloudFront (taken down after testing to avoid costs)

## Screenshots

### Live website (HTTPS)
![Live site](https://github.com/Aswinilokeshwaran/aws-s3-cloudfront-static-website/blob/3d5a6d298627b8a5509dafccf51546fc2aa2608d/1-live-site.png.jpeg)

### S3 bucket files
![S3 bucket](screenshots/2-s3-bucket.jpeg)

### Block public access and bucket policy
![Block public access](screenshots/3-block-public-access.jpeg)

### CloudFront distribution
![CloudFront](screenshots/4-cloudfront-general.jpeg)

### CloudFront origin (S3)
![Origins](screenshots/5-cloudfront-origins.jpeg)

## What I learned
- How to keep an S3 bucket private and serve it safely through CloudFront
- S3 file names are case-sensitive
- CloudFront caches files, so updated files can take time to show (an invalidation clears the cache)
