Source code for my Resume

Built using https://jsonresume.org.

Want to see it live? [Click here](https://registry.jsonresume.org/Alexandru-Dumitru)

For development:

1. Clone
2. Edit `resume.json`
3. `npm run test` to run schema validation (Intellisense should take care of this)
4. `npm run dev` to develop in watch mode
5. `npm run build` to generate a pdf version of the CV

6. Update [gist](https://gist.github.com/Alexandru-Dumitru/7bcbed1ff82c27a3a491799615882001) with the content of `resume.json`

> :warning: If the pdf is not rendered properly (fit in page), play with settings of `page.pdf()` (line 110) in this file `node_modules\resume-cli\lib\export-resume\index.js`
- I removed `format: letter` and used `width:length` size. FYI, `format: A4` didn't work :worried:
```
width: 2100,
height: 2970,
```
- is what saved me :grin: