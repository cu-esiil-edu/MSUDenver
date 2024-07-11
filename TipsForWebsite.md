**Tips for Website:**



1. Begin a document write-up of your website - at the same time you are creating the presentation slides.  
    * You can assign 1 or 2 people or the same people who are doing a specific part of the research slides can do it.
    * Consider who your audience will be: citizens of the area, students, scientists, etc.
    * Include headings and sub-headings in the write-up as a website would have.  Titles should capture the main point/so what? of that section.
    * Write out what would be narrated in the presentation, but you can include more detail.  (Make it concise enough that people will read it. 🙂)
    * Include a sample of code in the website, with a link to the code if you want it to be reproducible.  Google collab can be saved as Github code and vice versa.
2. Create your webpage space with url in [github.com/cu-esill-edu](github.com/cu-esill-edu)
    * People working on the webpage, may need to ask Nate and Elsa to invite you to join.  You will need to give them your GitHub username and then you’ll receive a link in email.  Click and you're in!
    * Create a new repository with the format: github.com/cu-esiil-edu/MSUDenver-nameOfYourProject2024.
      	*  choose "make it public"
      	*  check "add a README"
      	*  MIT license should be fine or choose another
    * Save a link to your page in the README of [github.com/cu-esiil-edu/MSUDenver](github.com/cu-esiil-edu/MSUDenver)
3. Pick a theme:
    * Make sure it is a GitHub supported theme.  (You do not need to download Jekyll or Ruby so don’t go down that rabbit hole.  The point of GitHub is that it has those supports already built in.)  GitHub supported themes don’t have to be from GitHub.  Here are some sites for theme searching:
        * [https://jekyllthemes.io/free](https://jekyllthemes.io/free)
        * [https://jupyterbook.org/en/stable/start/publish.html](https://jupyterbook.org/en/stable/start/publish.html) (these might be more complicated than jekyll)
        * [Supported themes | GitHub Pages](https://pages.github.com/themes/) (These are really simple.  They are designed for a minimal amount of information so don’t have navigation bars)
    * Find a real-world example of the theme being used with GitHub, not just on the demo page.  This is crucial as you can use code examples to help you build the page.  Google is a useful tool for this: “Website with ___ theme.”If there is not an example available, move on to a different theme.  One theme, just-the-docs that has already been used by the ESIIL Stars team is: [ESIIL Stars Syllabus](https://cu-esiil-edu.github.io/stars-2024/) and  [Syllubus GitHub Page](https://github.com/cu-esiil-edu/stars-2024).  A link to that theme is here: [just-the-docs theme](https://github.com/just-the-docs/just-the-docs/tree/main).
    * If you want to make sure your page can be tailored the way you want it, you can check the config.yml.  The config.yml is listed in the repository of the theme, along with readme and index, etc.
        * For example, if you want to be able to create and name navigation tabs, look for something like this in the config.yml folder: (To find this, click on the theme sample, then click on the GitHub link in the sample, and that should lead you to the GitHub folders page.  Then click config.yml.) 

             navigation:


                     - title: Home


                      url: /index.html


                    - title: About


                      url: /about


                    - title: Contact


                      url: /contact


			However, navigation tabs can also be built as individual pages.

		For this, you will want to look for a page heading that includes “nav” at the top of the page like this:
 
 
        		 layout: default


        		 title: Meet Our Team

	
      			 nav_order: 2


        The config.yml demo will have the word nav in it,  something like this:


        	nav_enabled: true



        * If you want to change the header photo, look in the config.yml for something like: 

    			#blog logo


          		logo: "/assets/images/df_logo.jpg"


          		float_logo: true # true, false (default)
          
          or:
          
				#blog cover


				cover: "/assets/images/cA4aKEIPQrerBnp1yGHv_IMG_9534-3-2.jpg"

        * If a site doesn’t have the functionality that you want, don’t pick it.  You likely don’t have time to build it in. 
    * After you pick a theme, in your webpage repository on GitHub, add the theme name to the config.yml.	
        * If it is a GitHub theme, use the format

            theme: username/name of theme

        * If it is a Jekyll, jupyter, or other theme, use 

            remote_theme: username/name of theme


            For example, your config.yml file might start with something like:


            Title: Project


            description: Water Quantity


            remote_theme: just-the-docs/just-the-docs

4. Convert the write-up to code.  There is an easy way: 
    * Within Google Docs:
        * Extensions > Add-ons > Get add-ons
        * Choose Docs to Markdown
        * Now you can convert your document by highlighting the text you want to convert and then by going to Extension > Docs to markdown > convert
        * Images will need to be be converted individually: see below.
    * Within Microsoft Word
        * File > Get Add-ins and search for Markdown.  Markdown or Easy Syntax Highlighter are some examples that might work similarly to Docs to Markdown.
    * Adding images
        * On GitHub, create a folder to store images and name it img.  Example: cu-esiil-edu<span style="text-decoration:underline;"> </span>/MSUDenver-DineWaterQuality2023/img
        * Within this folder, create a folder titled .keep.  This will allow the img folder to save.  Commit changes.
        * To add an image, first, save it on your computer.  Then, in GitHub, go to Add file > create new file and add image that is saved on your computer.  Commit changes.
        * Go back into the image, right click on the image, and select copy image link.  
        * Paste image on webpage using Markdown.

Congrats!  Now you can build your webpage!

Many thanks to Nate and Dr. Culler for lots of these tips!
