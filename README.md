# npx tailwindcss-candidates

A fork of Tailwind CSS with added functionality to output all detected Tailwind CSS classname candidates. This feature allows you to see which classnames are recognized during the build process, aiding in debugging and understanding which classes Tailwind is using.

## Badges

![npm](https://img.shields.io/npm/v/tailwindcss-candidates) ![npm](https://img.shields.io/npm/dt/tailwindcss-candidates)


## Usage

Use this fork just like Tailwind CSS. In addition to generating the final CSS output, it will also provide a list of all classname candidates it detected, which can be used for debugging or building a safelist.

```bash
npx tailwindcss-candidates -i ./src/styles.css -o ./candidates.txt --content "./src/**/*.{html,js,jsx,ts,tsx}
```

Given an input CSS file, `src/styles.css`:

```css
@tailwind components;
@tailwind utilities;
```

This will generate `candidates.txt`:

```txt
sr-only
fixed
absolute
relative
```



## License

This fork follows the [MIT License](LICENSE) in alignment with the original Tailwind CSS project.
