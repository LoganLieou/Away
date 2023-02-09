## Away

A really busted modern latex editor.

This came to me while using notion and I was like this is really pretty too bad
all the latex editors are doo doo pee pee water. So I decided this sounds
really easy so I wrote my own.

As of right now the only thing that this does is allow you to edit text, so this
is still a work in progress below I underline some features and how to achieve
these features

## Features and How to Implement

- Reading and Writing Files - file io with electron to local device bc you can't
do this from react as it expects you to be in the web browser, I mean you could
probably read files with a drag and drop but I'm not entirely sure how to write
files, there's a really scuffed way to do this as well by implementing an api
from the application to the local machine you can write files by listening for
some request
- Various latex templates documents etc. just load a bunch of templates so ez
this is what overleaf does anyway it's community sourced but for here I can just
have some basic templates that I use since the use case seems to be personal
- pdf viewer, it's a browser lol just view the pdf you can use PDF.js this
should just be built into electron I'm p sure

## Usage

there's 3 commands in `package.json` and here's how they work since I any %'d
this project the whole thing is really shit

`npm run dev` - normal in browser react live server

`npm build` - builds the electron app so you can `npm run prod`

`npm run prod` - runs the electron app is not live must be built to see changes
