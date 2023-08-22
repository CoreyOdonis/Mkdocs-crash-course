# TABLE OF CONTENT
- Introduction to MKDocs 
    <ul>
    <li>What is MKDocs?</li>
    <li>Why use MKDocs?</li>
    <li>What can MKDocs be used for?</li>
    </ul>

- Getting started with MKDocs
    <ul>
    <li>Installing MKDocs</li>
    <li>Creating a new MKDocs site</li>
    <li>Writing your documentation</li>
    <li>Hosting your documentation</li>
    </ul>

- Customizing your MKDocs site
    <ul>
    <li>Themes</li>
    <li>Plugin extensions</li>
    </ul>

- Summary


## What is MKDocs
MKDocs is a documentation tool that processes Markdown files into static website. It is an open-source python-based static site that focuses on speed and simplicity. Documentation source files are written in Markdown file format and configured with a YAML configuration file.

## Why use MKDocs
MkDocs offer several key features that makes life easier for users, some of which are:

- Speed and simplicity: It is quite fast and easy to use, as it can be set up within minutes and you don’t have to learn a complex markup language to get started.

- Themes: A quick glance at the MKDocs official website and you are provided with good looking built-in themes to get you started, or you could customize your own theme depending on what look and feel you want your documentation to have.

- Plugins: The presence of a large array of plugins provided by MKDocs to speed up your process makes it the best fit for documentation. Some of the plugins available are pdf-export, table reader, auto links, redirects, and Marcos.
    
- Preview your site as you work: It provides you a built-in dev-server to preview your documentation as you write. It also auto refreshes your browser whenever you save your changes.
    
- Ability to host your documentations anywhere: You can host your documentation to a variety of platforms such as GitHub, GitLab, AWS S3, Netlify, Vercel etc.
    

## What can MKDocs be used for
- Product technical documentations: It can be used to create documentations for language libraries and frameworks. This helps software engineers provide clear and concise documentation on their codebase for third-party.
    
- Educational resources: It is suitable for building an educational resource base which could range from reference materials, teaching resources and step-by-step guide for various tasks.
    
- Generating marketing materials: MKDocs can be used to showcase case studies and success stories on how your product or services help or have helped people in the past. It can also be used to create informative whitepapers as well as press releases in a structured and organized manner.
    
- API Documentation: It can be used to create documentation for APIs, so developers can understand what the API entails and how to use it in their projects.
    
- User manual: It can also be used to create guides, products and applications, which lets users understand how to use the software.
    
- Open-source projects: It is common to use MKDocs to create documentation that enlightens contributors as well as potential users of the product to understand the purpose of the project, and how to be a contributor.
    
- Creating a personal website or blog: While MKDocs are primarily designed for documentation purposes, it can also be used to curate contents for a personal website using markdown language. You can easily organize your content using the in-built hierarchical folder structure, customize the themes provided by tweaking the CSS or layout to provide better aesthetic, and you can host it on a plethora of free hosting website platforms.
    

## How to install MKDocs
MKDocs requires you to have a recent version of python and the python package manager `pip` to be installed on your system.

- To check if you already have these installed; if you use windows, open the Run menu with Windows Key + R, then press `Enter` to open the regular command prompt, then type `python` and hit Enter once your command prompt is opened. If you use a mac, press Command + Space bar on your keyboard, then type in terminal, then type `python` and hit Enter .

- To check if you already have these installed, open your command prompt `cmd` and input the code below. 
    ```pip --version```
    
- To install pip for the first time, then run the following command to install it. 
    ```Python get-pip.py```
    
- To upgrade your python package to the latest version, run this command. 
    ```Pip install --upgrade pip```
    
- Having done the steps above, it is now time to install MKDocs, to do this, run the command below.
    ```Pip install mkdocs```

- However to check that everything worked as it should, run ```mkdocs –version.``` in your Vscode terminal.<br>
You should also install mkdocs materials using this command
     ```pip install mkdocs-material```
    

Now you have your MKDocs installed


## Creating a new MKDocs site

- Create a folder on your system and give it a short name, then launch your IDE. <br>
we would be making use of Vscode for this article.
    
- as soon as your vscode is opened, type this shortcut on your keyboard `Ctrl+K Ctrl+O` to open folder. for mac users, use `Command+k command+O`. afterwards, navigate to the folder you created in the first step and select it.
![Vscode Home](../../img/vscode%20home%20screen.png "Here is your onboarding screen in Vscode")
    
You could also do this to open your folder. once your Vscode is opened, click `open folder`,and then navigate to where your folder is located and select it.
![vscode](../../img/home%20screen.png)

- Click the menu bar and then navigate to `New terminal`
![vscode](../../img/hamburger%20menu.png "open your Vscode terminal here")

- create new project in your terminal using the command `mkdocs new [dir-name]. It should be noted that dir-name in the command line is the name of your project so you could give it any name, just ensure you put a dash in between each word.

- You will notice 2 files have been created in your mkdocs folder.
![vscode](../../img/mkdocs%20file%20created.png "New MKDocs folder has been created successfully")
    
- Now your mkdocs file has been created

## Writing your documentation
MKDocs uses the python-Markdown library to render Markdown documents to HTML. You still
write in the regular Markdown language but it would be placed somewhere in your project
directory. The file would be named docs and will be placed alongside the mkdocs.yml
configuration file.



- To start the live-reloading docs server. use this command in your terminal
    ```mkdocs serve```

- To build the documentation site. use this command in your terminal
    ```mkdocs build```

## Hosting your documentation
You can deploy your docs on GitHub by making use of GitHub Pages to host the documentation
for your project. Once you checkout the primary working branch master of the git repository.
Run the command below.
```mkdocs gh-deploy –clean```

MKDocs will help you build your docs following the way you’ve set your docs

## Themes
You can access a couple of built-in themes as well as various third party themes, all of
which can be customized to your preference using CSS or Javascript. To use a theme that
is included in your MKDocs, add this to your mkdocs.yml config file.
`theme: readthedocs` <br>
You are to replace readthedocs with any of the built-in themes available


## Plugin extensions
To install third party plugins, you must determine the appropriate package name and install it
using pip. Lets assume we want to install *pdf-exports* plugin, do this in your terminal
```Pip install mkdocs-pdf-exports-plugin```
<br>
Then configure the plugin in your mkdocs.yml configuration file like this.
```Plugins:
     Search
```

You can then generate the PDF by running the following command.
```mkdocs pdf```


## Conclusion
If you are looking to create documentation for your software project and you want a platform that is easy to use, flexible, reliable, SEO-friendly, free and open-source, while supporting continuous integration. MkDocs gives you that freedom and control to create clean and professional documentation.