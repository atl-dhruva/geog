The purpose of this HTML file is to display Annexation Reports filed with the Georgia Department of Community Affairs prior to the GIS file validation requirements introduced on September 1, 2025.

The project folder contains two data files that are referenced by the HTML file:

  - "georgiacounties.csv" is used to generate a the selection list of Counties that appears in the main view.
 
  - "historicannexations.csv" is used to populate the data table that appears after a County is selected.

  - Both of these .csv files can be updated as needed. Simply update the data in GitHub & press "Commit Changes".
 
  - It's important to keep them in the same project folder as "index.html", otherwise the data won't load properly.

**The data in this file was collected on April 25th, 2025.** I intend to update "historicannexations.csv" with April 25 to September 1 data the day before the new Annexation Reporting system launches on September 1, 2025. I will update this README file as necesseary to reflect updates.

This HTML site will be shared via GitHub Pages, then added as an iFrame to the DCA's Annexations Dashboard located within DCA's Annexation Reporting & Resources ArcGIS Hub site.

**ADVANCED:**

If you wish to test out updates to the HTML file before committing changes, follow these steps.

**SECTION 1 - INSTALLING PYTHON**

I'll walk you through installing Python in Section 1. If you already have Python, skip to Section 2.

  1. Open a Command Prompt on your computer. You can use your Windows Search to open it - search for "Command Prompt".
   
  2. Type "python" (no quotes) in your Command Prompt. Press Enter.
   
  3. If you don't have Python, a Windows Store download window will pop-up. Use that to download Python.
   If you already have Python, you'll instead see a version number returned in the Command Prompt output.

**SECTION 2 - EDITING, PREVIEWING, & TESTING THE INDEX.HTML FILE**

You will need to set up a Local HTTP Server on your computer to test the .html file. Simply opening the .html file with your internet browser won't work due to browser-based restrictions on loading .csv files. If this is new for you, don't worry - it's easy! You only need to use one line of Python code. 

  1. In GitHub, download the "geog/historicannex" folder containing the .html file, two .csv files, and this README file.
     Save it to your computer's Documents folder.
     
  2. Open the "historicannex" folder on your computer using Windows File Explorer.
     
  3. In the Search Bar at the top of your File Explorer, type "cmd" (no quotes) and press enter to open the command prompt.
     **(Make sure the command prompt is in the "historicannex" folder.** You should see its name in the command prompt.)

  4. Enter the following command in the Command Prompt: "python3 -m http.server -b 127.0.0.42 8080" (no quotes)
     
  5. Open a web browser and enter the following (as if you were trying to go to a website):
     "http://127.0.0.42:8080" (no quotes).

**You should see the Historic Annexation Table web app in your browser at this point.**

  6. Navigate back to your Windows File Explorer folder called "historicannexations"
 
  7. Right-click "index.html" and choose "Edit in Notepad". (If you don't see this option, try "Open with > Notepad")
  
  8. You can directly change the HTML, CSS, or JavaScript in this file.
  
  9. Press "Save", then refresh your browser at "http://127.0.0.42:8080" to preview the edits.
  
  10. When you're happy with the edits, use GitHub to suggest the modifications to atl-dhruva using a pull request.

**What to do if atl-dhruva is not available to push updates**
  
  11. Feel free to upload a clone of the modified "historicannex" project folder to your own account.
  
  12. To make the HTML page viewable on DCA's Annexations Hub, you need to share your project using GitHub Pages.
  
  13. You then need to use the URL of your Github Page as an iFrame in the Annexations Hub.
  
  14. There should already be an iFrame with atl-dhruva's GitHub Pages link; just substitute it for yours.

**Contact**
gis@dca.ga.gov
