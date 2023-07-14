# Nextjs - Js/Ts Snippets

## Description

This extension provides code snippets for common JavaScript and Next.js patterns to enhance your development workflow. It includes snippets for logging to the console, creating components, data fetching, importing images and fonts, and more.

## Features

- Simplify your coding with ready-to-use code snippets
- Improve productivity by automating repetitive tasks
- Support for both JavaScript and TypeScript languages
- Includes snippets for common Next.js patterns

## Commands

| Command  | Description                                                                |
| -------- | -------------------------------------------------------------------------- |
| `log`    | Print message to the console                                               |
| `nafc`   | Create a function for Page.js                                              |
| `nal`    | Create a basic Layout                                                      |
| `nafcdf` | Create a Data Fetching page                                                |
| `<Image` | Image component allowing you to easily display images without layout shift |
| `impi`   | Import Image component from next/image                                     |
| `impf`   | Import font from next/font/google                                          |
| `impfd`  | Import font from next/font/google with declaration                         |
| `implf`  | Import local font                                                          |
| `implfd` | Import local font with declaration                                         |
| `impl`   | Import Link from next/link                                                 |
| `<Link`  | Link component allowing you to navigate within your application            |

## Usage

To use the snippets, follow these steps:

1. Install the extension in Visual Studio Code.
2. Open a JavaScript or TypeScript file.
3. Start typing one of the commands listed in the table above.
4. Select the desired snippet from the suggestion dropdown or press Enter to insert it.

## Example Codes

### Print message to the console

```javascript
console.log("Hello, World!");
```

### Create a function for Page.js

```javascript
export default function Page() {
  return <div></div>;
}
```

### Create a basic Layout

```javascript
export default function Layout({ children }) {
  return <section>{children}</section>;
}
```

### Create a Data Fetching page

```javascript
async function getData() {
  const res = await fetch("https://api.example.com");
  // The return value is *not* serialized
  // You can return Date, Map, Set, etc.
  return res.json();
}

// This is an async Server Component
export default async function Page() {
  const data = await getData();
  return <div></div>;
}
```

### Image component allowing you to easily display images without layout shift

```javascript
<Image alt="Alt Text" src={src} placeholder="blur" />
```

### Import Image component from next/image

```javascript
import Image from "next/image";
```

### Import font from next/font/google

```javascript
import { Inter } from "@next/font/google";
```

### Import font from next/font/google with declaration

```javascript
import { Inter } from "@next/font/google";

const googleFont = Inter();
```

### Import local font

```javascript
import localFont from "@next/font/local";
```

### Import local font with declaration

```javascript
import localFont from "@next/font/local";

const myFont = localFont({ src: "./my-font.woff2" });
```

### Import Link from next/link

```javascript
import Link from "next/link";
```

### Link component allowing you to navigate within your application

```javascript
<Link href="/go-to">Go to</Link>
```

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request to the [GitHub repository](https://github.com/nshibu/nextjs-js-ts-code-snippets).

## License

This extension is released under the [MIT License](https://opensource.org/licenses/MIT).

Feel free to modify the content of the `readme.md` file to match your extension's details, usage instructions, and any additional information you want to provide.
