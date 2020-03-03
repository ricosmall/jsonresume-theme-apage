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
```

## Example

[http://themes.jsonresume.org/theme/apage](http://themes.jsonresume.org/theme/apage)

## License

Available under [the MIT license](http://mths.be/mit).
