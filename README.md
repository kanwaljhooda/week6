# Week 6: Netlify Dev Install and Test

1. This step was part of the pre-work before Week 1, but if you haven't already, install node.js – https://nodejs.org and choose the "Current" version. Open the installer and complete the steps using defaults only (note: if prompted to install "Tools for Native Modules", skip it; do not check the box, just click "Next").
1. If you haven't already done so, create a new repository in your GitHub account by selecting "Use this template"; call the new repository "week6" and clone/open the new repo in VSCode.
1. In VSCode, open a new Terminal window via the menu bar -> Terminal -> New Terminal. In the Terminal, ensure that Node was successfully installed by typing `node -v` and hit Enter. A version number (e.g. `v15.x.x` or similar) should be returned.  
1. Install the Netlify developer tools. In the VSCode Terminal, type `npm install netlify-cli -g` and hit Enter. It should take a couple of minutes. Afterwards, type `netlify -v` to ensure the installation was successful.  The installed tool and version number (e.g. `netlify-cli/3.x.x` or similar) should be returned.  If it isn't, ask for help in Slack or during office hours.
1. Make sure your VSCode Terminal is in the `week6` project directory – on Windows, the prompt should tell you what directory you're in; on Mac, you can type `pwd`. It should return something similar to (Windows) `c:\code\week6` or (Mac) `/Users/username/code/week6`. Type `npm install` to install the rest of the dependencies (libraries of code) needed for the project.  You should get a progress bar (sometimes it takes a while), and in the end, you should see "found 0 vulnerabilities" in the output.
1. Last command - type `netlify dev`. In the VSCode Terminal, you should see something like *Server now ready on http://localhost:8888*. If asked to give VSCode control over Chrome, click Yes. A browser window should pop up with the contents of `index.html`.

**You'll 💯 know if the setup worked - the success page is very obvious.** Make sure you're seeing the success page from doing `netlify dev` and on `http://localhost` and not because you double-clicked on `index.html`!

Now that everything is installed and working, you can end the terminal session by typing the keys CTRL+C in the terminal window (Windows only: if prompted to "Terminate Batch Job?", type "Y" and hit Enter).  This will stop the Netlify Dev server.  You're ready for class!

## For Windows users only

If any of these commands don't work and you're not seeing the output specified in each step/don't see the success page, try one of two fixes:

- In your Terminal window in VSCode, there's a little dropdown; select the option to "select a default shell". Select cmd and close and re-open the Terminal window.
- If that doesn't work, do everything outside of VSCode using the Command Prompt that's built into Windows: Start Menu -> type `cmd`. Then change into the week6 directory typing `cd \code\week6` (`cd ` with a space, then the file path to your week6 folder), and then go through the instructions above.