# PhotoEditor
A GUI application written in PHP using wxWidgets (via wxPHP) and ImageMagick (via MagickWandForPHP)

Title: Photo Editor

Version: 0.99.0

Author: Dave Kimble

Date: 8 January 2015


Requirements: 

You must have installed:

	PHP 5.4.29	 			v5.5.9 is backwards compatible 
	
							http://php.net/downloads.php 
								      	
	wxWidgets 3.0.0+ 		https://github.com/wxphp/wxphp/wiki
	
							svn checkout http://svn.wxwidgets.org/svn/wx/wxWidgets/tags/WX_3_0_0 wxWidgets
							      	  
	ImageMagick 6.9.0+ 		https://subversion.imagemagick.org/subversion/ImageMagick/branches/ImageMagick-6.6.0/www/install-source.html
	
							http://www.imagemagick.org/download/
							      		
	wxPHP 3.0.0.2+      	https://github.com/wxphp/wxphp/wiki
	
							git clone https://github.com/wxPHP/wxPHP.git wxphp
							      		
	MagickWandForPHP 1.0.9+	http://magickwand.org/
	
							svn co https://www.imagemagick.org/subversion/MagickWandForPHP/trunk MagickWandForPHP
								      	

Installation: 

1.	Download the files to your filespace: git clone https://github.com/davekimble2/PhotoEditor /path/to/PhotoEditor

2.	Edit .../PhotoEditor/photoeditor.wxphp configuration section to set your default path/folders, etc

   
Running:

3.	Run with php /path/to/PhotoEditor/photoeditor.wxphp

  	or (for Ubuntu 14.04)
  	
  	edit the photoeditor.desktop file for file paths
  	
  	copy the file to ~/.local/share/applications/ 
  	
  	and launch from the main menu.
  	
4.	The main window always runs maximized, 

  	you can hide the main window by clicking the minimize icon or the tray icon.
  	
	  You can show the main window by clicking the tray icon again.
	  
5.	The Toolbar can be hidden by clicking the Hide button.

	  You can show the Toolbar again by single left click anywhere on the main window.
	  
6.	The Exif Properties button will show the original image's Exif data,

	  which will be included on saving.
	  
   
Known issues:

1.	Runs as Always On Top (this appears to be a platform-dependent bug in wxWidgets)

2.	Does not respond to f11 key, so doesn't run FullScreen on Ubuntu 14.04

3.	Does not create a taskbar icon in Ubuntu 14.04
