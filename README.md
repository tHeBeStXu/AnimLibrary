# AnimLibrary
Animation Curve Library
	    
This is a Anim Curve Library tool for animation work.	        
It is Pyside2 version only for Maya2017.
Before using the script, you need to make true that your maya setup is OK.       		    
You can use it to export and import animation curve. For management, you can create, expand, collapse, rename and remove pose library folder.		

# Preparation:
1. Make ture you have installed the imageio, Pillow and PIL packages for your Python27.
2. Because Maya use a custom compiled Python version, you need to compile the Pillow for your maya version.         
   Here is a tutorial for how to compile the Pillow for Maya2017 and Maya2018.
   https://around-the-corner.typepad.com/adn/2017/05/how-to-build-pillow-on-windows-with-maya-2017.html
3. You can also download the compiled Pillow/PIP packages for Maya2017.   https://drive.google.com/drive/folders/0B5n3XnEYY_bVN1d5QWFiSUhGMG8?usp=sharing   
   After you download the packages, unzip, copy and paste the packages to the proper directory.     
   (i.e. unzip Pillow.4.1.Python2711.VC2012.zip, copy the unzip file and paste it to Maya2017/Python;       
         unzip openjp2 (1).zip, copy the unzip file and paste it to PIL in Maya2017\Python\Lib\site-packages)

# How to install:
1. Download the project file and unzip it somewhere in the computer, make ture to remember the directory of the unzip file location.		
2. Open Maya 2017 and open script Editor		    
3. New a Python tab, and enter following script 		    

Dir = 'X:\WHERE\YOU\PUT\THE\FILE'		    
pythonLib = 'X:\WHERE\YOU\PYTHON27\INSTALL\site-packages'                       
import sys		

if Dir not in sys.path:		
    sys.path.append(r'X:\WHERE\YOU\PUT\THE\FILE')      
if pythonLib not in sys.path:
    sys.path.append(r'C:\Python27\Lib\site-packages')
  
import AnimLibrary

from AnimLibrary.UI import Main_UI
reload(Main_UI)

ui = Main_UI.MainUI()    

# How to use:
You can go to: https://www.bilibili.com/video/av44938064/ and watch the video.
# Bugs:
If you find any type of bugs, please e-mail me at: 328665042@qq.com.    
    
If you like, please STAR this repository. Thank you very much.    

# Future
I will compile some packages for Maya2018 Python and hope it will make your life easier.
