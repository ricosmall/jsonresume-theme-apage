# jsonresume-theme-apage

This is a theme for [JSON Resume](http://jsonresume.org/), it's responsive for multi screens, also trying to fit all infomation in a print page.

## Getting started

1. To get started with theme development, this is what you'll need:

   - [node.js](http://howtonode.org/how-to-install-nodejs)
   - [npm](http://howtonode.org/introduction-to-npm)

2. Then install [`resume-cli`](https://github.com/jsonresume/resume-cli):

   ```sh
   npm install -g resume-cli
   ```

3. Download or clone this repo to local:

   ```sh
   git clone https://github.com/ricosmall/jsonresume-theme-apage
   ```

4. Create a `resume.json` file:

   ```sh
   cd jsonresume-theme-apage
   resume init
   ```

5. Serve your file with the theme:

   ```sh
   resume serve
   ```

## Special Features

### Language Support

Current support chinese and english. By default, use `process.env.LANG` to get your locale. For example, if your computer language is chinese, will automatically set language to chinese when rendering.

You can also manually define it when using command `resume`, for example, if you want english support, just run like below:

```sh
# serve
LANG=en resume serve

# export
LANG=en resume export resume.pdf

# for those node with the Lang of en, you can use the following to render chinese resume
LANG=zh resume serve
```

### Special Chinese Support

1. You can add extra fileds in `basics`

   ```json
   {
      "basics": {
         "sex": "男",
         "age": "24",
         "workYears": "3年经验",
         "educationLevel": "本科",
         "avatar": "https://avatar.com/yourname.jpg"
      }
   }
   ```

   And those fields will display at the top of resume page, see [the demo](https://ricosmall.github.io/jsonresume-theme-apage/chinese.html).

2. You can also add extra filed `summary` in json file

   ```json
   {
      "basics": {},
      "summary": [
         "拥有俄克拉荷马大学和斯坦福大学的学位。",
         "在开始 Pied Piper 之前，在 Hooli 担任兼职软件开发人员。",
         "工作重点是应用信息论，主要是优化长度受限和自适应变体的无损压缩方案",
         "非工作兴趣范围很广，从量子计算到混沌理论。"
      ]
   }
   ```

   And the field will display at the bottom of resume page, see [the demo](https://ricosmall.github.io/jsonresume-theme-apage/chinese.html)

## Example

[jsonresume-theme-apage](https://ricosmall.github.io/jsonresume-theme-apage/)

## License

Available under [the MIT license](http://mths.be/mit).

