# tree

## `-I` 除外

~~~zsh
% tree . -I node_modules 
.
├── LICENSE
├── README.md
├── gatsby-browser.js
├── gatsby-config.js
├── gatsby-node.js
├── gatsby-ssr.js
├── package-lock.json
├── package.json
└── src
    ├── components
    │   ├── header.js
    │   ├── image.js
    │   ├── layout.css
    │   ├── layout.js
    │   └── seo.js
    ├── images
    │   ├── gatsby-astronaut.png
    │   └── gatsby-icon.png
    └── pages
        ├── 404.js
        ├── index.js
        ├── page-2.js
        └── using-typescript.tsx

4 directories, 19 files
~~~

複数除外:

- [tree command for multiple includes and excludes](https://unix.stackexchange.com/questions/61074/tree-command-for-multiple-includes-and-excludes)

~~~zsh
% tree -f -I "bin|unitTest" -P "*.[ch]|*.[ch]pp." your_dir/
~~~