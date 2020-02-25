## brad-hugo-cv
Brad Arnst's CV.

- based on Hugo (static website generator)
- a project for developing, building and deploying my CV

This is a static website, using Hugo at static website generator. It uses a fork of a Hugo theme from _cowboysmall_. [hugo-devresume-theme](https://github.com/cowboysmall-tools/hugo-devresume-theme). Which in turn was a Hugo port of [DevResume](//github.com/xriley/DevResume-Theme) - a resume/CV template designed Xiaoying Riley.

 It's a serverless, static website using Amazon AWS - S3, and AWS CloudFront as a CDN and to provide HTTPS/TLS.

 ### What's next?
 - The build is partially automated with Hugo. But, I'll add automate the conversion to the PDF file.
 - Deployment needs to be automated as well. Besides the upload to S3, the CloudFront objects have to be invalidated after the new deployment.
        
