## brad-hugo-cv
Brad Arnst's CV.

- based on Hugo (static website generator)
- a project for developing, building and deploying my CV

This is a static website, using Hugo at static website generator. It uses a fork of a Hugo theme from _cowboysmall_. [hugo-devresume-theme](https://github.com/cowboysmall-tools/hugo-devresume-theme). Which in turn was a Hugo port of [DevResume](//github.com/xriley/DevResume-Theme) - a resume/CV template designed Xiaoying Riley.

 It's a serverless, secure, static website. It runs on Amazon AWS, using S3 as the storage/website and Amazon CloudFront for the CDN and to provide HTTPS/TLS.
 The actual content of the website is all in the config.toml file. The frontmatter contained in this file is injected (when Hugo is run) into various partial HTML files, such as experience.html, skills.html, etc. It is styled from the Bootstrap scss files and from a devresume.scss file from (see above) the original developers of the theme. The CSS is generated along with the HTML when Hugo is run.
 
 Some of the frontmatter, in the config.toml file, can be formatted using Markdown. The syntax is a bit limited. The whole process is not as straight forward as just a regular .MD Markdown file. It only works with some of the fields in the TOML file. Note: this is accomplished by using _Markdownify_ a Markdown processor built in to Hugo.

 Note: You can also use multiple lines within the config.toml file to format your TOML file for greater readability. For instance, if you have a longer paragraph you want to include, you can break up the paragraph into multiple lines instead of having a long line in your text editor. This is an aspect of the TOML specification that I did not know about before this project. Start with three quotation marks, and multiple lines and end with three marks. See [TOML Specification](https://github.com/toml-lang/toml).

 View website here: [Brad Arnst CV](https://cv.nexusseven.com).


 ### What's next?
 - The build is partially automated with Hugo. But, I'll add automate the conversion to the PDF file.
 - Deployment needs to be automated as well. Besides the upload to S3, the CloudFront objects have to be invalidated after the new deployment.
        
