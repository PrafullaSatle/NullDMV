To use Tailwind CSS you must have to run this command in CLI:
"tailwindcss -i ./src/input.css -o ./src/output.css --watch"

For the convinience you have set the shortcut for above command, thus use only:
npm run tcss

TO make any changes in shorcut you need to change package.json
"scripts": {
  "tcss": "tailwindcss -i ./src/input.css -o ./src/output.css --watch"
}

To stop the terminal from watching and making changes y=just write "Ctrl+C" in command line.

When you are going to use tailwindcss the rel link will be different for different folders

(1) If you wanted to use it in 'src' folder then it will be as:
<link href="./output.css" rel="stylesheet">

(2) If you wanted to use it in "Tailwind Project" folder then it will be as:
<link href="../output.css" rel="stylesheet">

(3) If you wanted to use it inside other folder which is not subfolder of 'src' then it will be as:
<link href="../src/output.css" rel="stylesheet">