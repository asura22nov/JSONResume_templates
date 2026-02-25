# JSONResume_templates
building resume using JSON Resume Standards

https://jsonresume.org/

Had a copy of my resume in Reactive Resume. Export .json
Used Gemini to convert reactive resume .json into JSON Resume .json standard schema

#softwares on windows
https://nodejs.org/dist/v24.14.0/node-v24.14.0-x64.msi
npm install -g resume-cli

#JSON Resume commands
resume --version
resume init


#JSON Resume themes 
npm install jsonresume-theme-professional
npm install jsonresume-theme-standard
npm install jsonresume-theme-spartacus
npm install jsonresume-theme-elegant
npm install jsonresume-theme-flat
npm install jsonresume-theme-kendall --> only this worked out

#html rendering
resume serve --theme ./node_modules/jsonresume-theme-kendall  -r anand_resume.json

#JSON Exports
resume export anand_resume.pdf --format pdf --theme kendall -r anand_resume.json
resume export anand_resume_kendall.html --theme ./node_modules/jsonresume-theme-kendall  -r anand_resume.json
