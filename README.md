# ADUN CSS (adun.css)

This is my personal, lean CSS Framework or project starter template based on SASS (SCSS) and CSS Variables. This framework is heavily inspired by ACSS ([Automatic CSS by Kevin Geary](https://automaticcss.com/)).

## INSTALLATION

To use this CSS Framework, clone this repo or download the zip file and extract it. There are two versions:

i. SASS only - This is the version I use personally and it uses the Live SASS Compiler plugin to compile the SASS, and purgeCSS to clean up unused CSS in the final CSS output.

I chose this method because the SASS compiler used in PostCSS does not output colors as "hsl" and forces transparent variants to output as "rgba" too. I want my compiled colors to remain in hsl format.

To use this version, install [Live SASS Compile](). I have included a local setting for the plugin under ".vscode" folder. You can modify it to fit your project structure.

Also, delete `package-postcss.json` and `postcss.config.js`. It's optional but helps to make your project structure tidy.

ii. PostCSS and plugins - This is the best version if you don't mind your final colors to be in "hex" and "rgba" formats.

To use this version, delete `package.json`, then rename `package-postcss.json` to `package.json`.

Run `pnpm install` or `npm install`, then `pnpm start` or `npm start`.
