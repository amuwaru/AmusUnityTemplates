# Amuwarus Unity Templates
<img width="100" height="100" align="left" style="float: left; margin: 0 10px 0 0;" alt="icon" src="https://lh3.googleusercontent.com/proxy/AAQvHQWUGXHDCWFFPpt0XoWjf0v7xSxPz3OH4cbQb3PQ1ncHi2l_DpNCrfSQqtVNadb_QDj_-yoWnfzmaYbecxw6DXnUZxyBGmREvBx5J3Jg1Vifl2FNHlrDz3-BSFlgDPV1D_sPfg">

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)  
made by [amuwaru](https://twitter.com/amuwaru).  

## Table of Contents
- [Why? What's the point?](#reason)
- [Templates](#templates)
- [How to Install](#install)
- [Important notes and considerations](#notes)

## REASON
Everybody knows that when creating a new script, unity likes to load the default template.  
<img width="800" height="400" alt="example" src="https://forum.unity.com/attachments/before-jpg.332302/">  
This is okay for beginners, but for experienced developers, having to delete the help comments and more is just a very annoying nuisance.  
I know it doesn't take more than two seconds to do it...  But I'm very nitpicky about it and don't want to do the starting changes each time I create a script.  
Thus, I made my own template, and now I've realized that maybe there's someone out there that dislikes having to do the same probably...  
So, I made a buncho templates with different characteristics. Some more extensive than the others, and some barebones with just the necessary.  
Even though these templates are designed to be better and faster, some of you might find them even more disgusting than the original Unity template. Modify these templates to satisfy your needs or create your own.

## TEMPLATES
### Extended MonoBehaviour
- Adds UnityEngine.UI to create, reference and use UI elements.
- Element placement ordering aid using regions.
- Element access ordering aid using comments.
- Adds more MonoBehaviour "magic methods" for easier setup.
- The magic methods contain a one-liner comment for quick explanation.
- Class access defaulted to internal.
- Method curly brackets are closed and in the same line.

### Fast MonoBehaviour (Recommended)
- Absolutely nothing except for the class declaration and Start() and Update() magic methods.
- Removed any explanation comments over the magic methods.
- Class access defaulted to public.
- Curly brackets are opened and at the same height.

### Barebones Class
- Absolutely nothing. Just an empty class with default using dependencies.
- Class does not inherit from MonoBehaviour.
- Curly brackets are opened and at the same height.
- Class access defaulted to public.

### Signature MonoBehaviour ⭐
- My personal favorite.
- Adds more MonoBehaviour "magic methods" for easier setup.
- Removed any explanation comments over the magic methods.
- Class access defaulted to internal.
- Separator comments for elements, and a one-liner guide for access order.
- Method curly brackets are closed and in the same line. Class curly brackets are at the same height.

*And more templates to come if requested...*

## INSTALL
1. - Download the desired templates or copy their contents.  
2. - Go to ```<Unity Installation>\Editor\Data\Resources\ScriptTemplates```  
**Example:** ```C:\Program Files\Unity\Editor\Data\Resources\ScriptTemplates```  
3. - Rename the downloaded templates to the same names of the existing templates you'd like to overwrite respectively.  
**Example:**  
The file in the repo is called ```"ExtendedMonoBehaviour.cs"```.  
Rename it to ```"81-C# Script-NewBehaviourScript.cs.txt"```.  
If you copied the contents instead of downloading, just paste them inside the templates you'd like to overwrite, and save.  
4. - Launch Unity and create a new script using the Assets>Create context menu.  
5. - If you did the steps correctly, the new script will be created based on the new overwritten template.   
  
Remember you have to do this for each different Unity build you'd like to have the templates on.

## NOTES
- In some of the templates I added regions to show where the elements should be placed according to popular conventions.  
However the use of regions is an anti-pattern and is highly frowned upon. Please consider deleting them after you've ordered your file with them.
- In some of the templates I added extra MonoBehaviour magic methods. Consider removing all unused ones to avoid unnecessary calls.
- In some of the templates the class access is defaulted to internal instead of public (basically just public but only for the current assembly).  
I did this because I generally don't make code that communicates between multiple assembly .DLLs. But if you do, feel free to change it back to public if you want access from outside the assembly.
