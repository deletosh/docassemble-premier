# Setup
1. Clone this repo
2. Rename the `template` inside the `docassemble` folder to the name of project
3. Open the folder in VS Code and start editing the `yml` interviews in `docassemble/<new-name-from-step-1>/data/questions`

## Develop interviews offline (no-internet)
### Prerequisite
- [Install docker](https://docs.docker.com/get-docker/)
- If you're on Windows, [install and setup Cmdr]((https://jonathansoma.com/lede/foundations-2019/terminal/setting-up-cmdr-as-windows-shell))
- On Windows, [update VS Code to use Tabby](https://www.youtube.com/watch?v=ZM2srjrE-gs)
- [Install Python](https://realpython.com/installing-python/)
- Install docassemble command line app, [docassemblecli](https://pypi.org/project/docassemblecli/)
  - Open Tabby or Terminal and enter `pip install docassemblecli` (you need to have Python already installed)
  
### Start development
[See this first for the full context](https://docassemble.org/docs/development.html#cli)
- Open the folder you cloned from GitHub in VS Code or similar
- Start the local playground: run `docker-compose up -d` in your command line (on windows, run this on Cmdr. On Mac, Terminal)
- You can now access your local playground at [http://localhost](http://localhost)
- Run the package installer in the background: Open Cmdr or Terminal and run 
  - `dainstall --norestart --playground docassemble-<new-name-from-step-1>` 
  - then `dawatchinstall --playground docassemble-<new-name-from-step-1>`
