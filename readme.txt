october 24, 2021

C:\webdev\portfolio-react-simple>

simple portfolio website

from:
    Sonny Sangha, who does React tutorials on YouTube
    where he mostly builds clones of popular websites.
    https://github.com/sonnysangha/Resume-Portfolio-Starter-pack

change the info:
    public\resumeData.json
    public\images
    public\images\portfolio

local start:
    npm start

deployed:
    https://portfolio-react-simple.vercel.app/

note on the deployment:
    Sonny Sangha's instructions for deployment, in README.md, are for a 
    deployment to Netlify without using github. This deployment was done 
    but later taken down. It involves running 'npm run build' to create a 
    build folder which is then dragged and dropped into a space on Netlify. 
    To deploy to Vercel, I left the build folder in place (its presence doesn't seem 
    to effect the Vercel deploy), but needed to do the following:

      In the package.json under "scripts", you should have:
    		"build": "CI=false react-scripts build"
		    in other words, add 'CI=false' to what is already there

    With this small change to the package.json, I pushed to github and did 
    a normal Vercel deploy.  Vercel seems to run it own 'npm run build' during its 
    deploy.

    update:
        git add . 
        git commit -m "message" 
        git push
