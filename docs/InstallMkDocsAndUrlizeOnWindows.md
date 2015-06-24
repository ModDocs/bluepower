How to install MKDocs and Markdown-urlize on Windows
-------------------------------------------------------

Requirements:
- Python 2.7.x or 3.4.x : Both work. My advice if doing a fresh install : Python 3.4
- Administator Access to CMD

Links: 
- markdown-urlize: https://github.com/r0wb0t/markdown-urlize/archive/master.zip.

Procedure:

1. Verify what type of command structure you have to use. (Administrator)
	Some may have to use 'pip <Command>', while others may have to use 'python -m pip <Command>'
	Seems like users with Chocolatey installed can simply use 'pip <Command>' instead of calling the python module interpreter everytime. Not confirmed though
	
2. Install mkdocs: (Administrator)
	'python -m pip install mkdocs' OR 'pip install mkdocs' : Dependent on the command structure you have found out works in step 1.

3. Install markdown-urlize: (Administrator)
	You'll need to install from the zip of the Github archive. In my experience, simply trying to install from the current master (not zip version) caused errors.
	'python -m pip install https://github.com/r0wb0t/markdown-urlize/archive/master.zip' OR 'pip install https://github.com/r0wb0t/markdown-urlize/archive/master.zip'

4. Open a CMD in the folder where you have the mkdocs.yml file.
	Either open a normal cmd and navigate to that folder by using 'dir' and 'cd'. Or open a CMD straight from explorer: Shift-Rightclick in the folder you have the mkdocs.yml in and choose 'open commandprompt from here'

5. Run 'mkdocs serve'

6. Open your browser and navigate to '127.0.0.1:8000'