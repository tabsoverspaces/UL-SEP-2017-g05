#-------------------------------------------------------------------------------
# Copyright (c) 2015-2016 University of Luxembourg.
# All rights reserved. This program and the accompanying materials
# are made available under the terms of the Eclipse Public License v1.0
# which accompanies this distribution, and is available at
# http://www.eclipse.org/legal/epl-v10.html
# 
# Contributors:
#     Alfredo Capozucca - initial implementation
#-------------------------------------------------------------------------------

User Manual Latex Template 
===================================

What Is This?
-------------
The folder lu.uni.lassy.excalibur.myproject.usermanual.report contains a Latex project.
This Latex project contains the basic documents and information to write a (IEEE Std 1063-2001 compatible) user manual for a software product.


Prerequisites
--------------------------------------------------
a) Tools:
1. Third-party applications listed in this page:
http://messir.uni.lu:8090/confluence/pages/viewpage.action?pageId=3014662

2. Eclipse
https://www.eclipse.org/downloads/

3. TeXlipse eclipse plugin
http://texlipse.sourceforge.net/
The plugin can be directly installed from the Eclipse Marketplace



b) Workspace configuration:
1. The preferences related to the TeXlipse plugin have to be configured
1.a This configuration depends on your local OS and the folder where the TeX distribution is installed.
Usual Bin directory of Tex distribution for each platform is presented (adapt according to TeX distribution's year: i.e. 2014,2015,2016,...):
1.a.1 On Mac:  /usr/local/texlive/2016/bin/x86_64-darwin
1.a.2 On Windows: C:\texlive\2016\bin\win32
1.a.3 On Linux: /usr/local/texlive/2016/bin/x86_64-linux
1.b Go to the Eclipse Preferences -> Texlipse -> Builder Settings -> Latex Temp Files, and ensure that the extensions .glo and .xdy are in the list. 

2. The Excalibur Report library project (i.e. /lu.uni.lassy.excalibur.standard.report.libraries) must be present in your workspace.
2.a.1 This library project is part of the Excalibur Standard Libraries, which can be obtained from 
http://messir.uni.lu:8090/confluence/display/EXCALIBUR/Downloads
2.a.2 Download the .zip file containing the Excalibur Standard Libraries.
2.a.2 Unzip the file and import the project lu.uni.lassy.excalibur.standard.report.libraries into your workspace.
Note: if the Eclipse you are using has the Excalibur plugin already installed, then you can obtain the full set of
Excalibur Standard Libraries by doing:
File -> New -> Other, browse to find Excalibur -> Projects -> Standard Libraries Projects



How To Use The Project
--------------------------
You might want to use this Latex project to write the User Manual Document for your own software product. 
To do this:
1. Start Eclipse IDE.
2. Disable the option "Build Automatically" from the Project menu (if option is enable)
3. Import the Messir User Manual Document Latex project into your Eclipse workspace.
4. Go to project's properties-> Builders, and check the makeGlossaries builder is properly setup regarding your local Tex distribution installation. 
Usual configurations are presented below:
4.a On Mac:  /usr/local/texlive/2016/bin/x86_64-darwin/makeglossaries
4.b On Windows: C:\texlive\2016\bin\win32\makeglossaries.exe
4.c On Linux: /usr/local/texlive/2016/bin/x86_64-linux/makeglossaries
5. Enable the option "Build Automatically" from the Project menu 
6. That's all. 


From now on, every time you make and save a modification on a .tex file, the file user-manual.pdf is regenerated
Check the time stamp on the first page of the document to know when it was generated.



Happy User Manual writing. 



 
