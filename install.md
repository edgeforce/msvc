<font size="2" face="Verdana, Arial, Helvetica, sans-serif" color="#000000"><script language="JSCRIPT">function checkExpand( ) { if ("" != event.srcElement.id) { var ch = event.srcElement.id + "Child"; var el = document.all[ch]; if (null != el) { el.style.display = "none" == el.style.display ? "" : "none"; if (el.style.display != "none") event.returnValue=false; } } }</script>

## <a name="geninstall">Installation Notes</a>

© 1998 Microsoft Corporation. All rights reserved.

Other product and company names herein may be the trademarks of their respective owners.

_Installation Notes_ contains vital information about installing Microsoft® Visual Studio™ 6.0 -- Development System for Windows and the Internet, and its family of development products. Information in this file may apply to all or a number of the products shipped in the Visual Studio suite. This Readme updates information provided in the _MSDN Library Visual Studio 6.0_ documentation.

_Installation Notes_ is one of a "family" of Readmes shipped with the suite. All product Readme files reside at the root of Visual Studio compact disc 1\. These Readme files (install.htm, plus several others called readme_XX_.htm, where _XX_ signifies a product) use current Web technology so users can find and view their information quickly. They may be viewed with a Web browser, such as Microsoft® Internet Explorer 4, or in Notepad.

##### [How do I print all the available Readme files at one time from Microsoft Internet Explorer?](# "Click to expand or collapse.")

<div id="PrintingInstructionsChild" onclick="cl_script_data" style="display:none"><a name="#ieinstructions"></a>

> 1.  Open readme_XX_.htm, or install.htm, in Microsoft Internet Explorer.
> 2.  On the **File** menu, click **Print**.
> 3.  In the **Print** dialog box, set the printing options you want.
> 4.  Select **Print all linked documents** and click **OK**.

</div>

### Contents

> **Note**   Be sure all headings in the table of contents are expanded when you search this Readme for a topic. In this way, you will know when the search finds the topic among the TOC headings.

##### [Installation Instructions for Visual Studio Programs](# "Click to expand or collapse.")

<div id="InformationonFilesandProgramsShippedwithVisualStudioChild">

> [Installing Over Visual Studio Beta, Pre-Release, and Technical Preview Installations](#releaseversionoverbeta)

> ["Side by Side Installation": Installing Multiple Versions of Visual Studio 6.0 Products on the Same Computer](#sidebysideinstallation)

> [Warning When Installing on Dual-Boot Computers](#installingondualbootcomputers)

> [Installing Visual Studio from a Shared CD Drive](#installationonsharedcddrive)

> [Let Microsoft Internet Explorer Setup Finish Before Proceeding with Visual Studio Installation](#letiefinish)

> [When Microsoft Internet Explorer Setup Installs Older Versions of MDAC Files](#ieinstallsoldmdacfiles)

> [Special Installation Instructions for Computers with Non-U.S. Versions of Microsoft Windows NT 4.0 and Microsoft Internet Explorer](#nonusnt40)

> [BiDi Systems Must Have Localized Version of Internet Explorer 4.0 SP 1 Before English Visual Studio 6.0 Is Installed](#localizediespneededforenglishvs)

> [When the Installation Wizard Looks for A Web Publishing Wizard Disc](#webpublishingwizarddisc)

> [Installing Client Tools and Server Components After Visual Studio 6.0 Products Are Installed](#installingclienttoolsafterinstallingvs)

> [How to Contact Technical Support](#howtocontacttechnicalsupport)

</div>

##### [Installing Server-Side Components](# "Click to expand or collapse.")

<div id="ServerSideSetupsChild">

> [Minimum Requirements for Installation and Operation of Server-Side Components](#minimumreqsforserversideinstall)

> ["Setup Already Running" Message Shows Up During Installation of Server-Side Components](#setupalreadyrunning)

> [Installing Server Components on Windows 95](#servercomponentsonwin95)

> [Known Compatibility Issues with SQL Server 6.5 and Windows NT Option Pack 4.0](#sqlandwinntop)

</div>

##### [Configuring for Debugging](# "Click to expand or collapse.")

<div id="configuringdebuggingChild">

> [For ASP Debugging, Install IIS Patch After Installing BackOffice](#iispatchforaspdebugging)

> [Using SQL Debugging Services on a Computer with SQL Server 6.5 and Visual C++ 5.0 or Higher Installed](#sqldebuggingoncomputerswithsql65andvc5orhigher)

</div>

##### [Issues Specific to Windows 9_x_ Computers](# "Click to expand or collapse.")

<div id="RelatedtoWindows95ComputersChild">

> [Windows 95 Registry Size: 64 KB Limitation May Cause A Warning During Visual Studio Installation](#windows95registrysize)

> [Disable Autologon Before Running Visual Studio 6.0 Setup](#whenautologonisenabled)

> [An Internet Connection Dialog Box May Appear at Startup of Windows or Other Applications](#internetconnectiondialog)

> [Installing Server Components on Windows 95](#servercomponentsonwin95)

> [For ASP Debugging on Windows 95/98 Computers, Install IIS Patch After Installing BackOffice](#iispatchforaspdebugging)

> [Installation Wizard May Not Restart After PWS Is Installed on Windows 95 Computers](#resumingsetupafterinstallingpws)

> [Installing Microsoft FrontPage 98 Extensions on Some Windows 95 Computers](#frontpage98onwin95)

</div>

##### [Notes Impacting Other Installed Programs](# "Click to expand or collapse.")

<div id="RelatedtoOtherProgramsChild">

> [IISAM Exchange Driver Will Fail if Microsoft Exchange or Microsoft Outlook Is Not Already Installed](#iisamexchangedriver)

</div>

##### [Issues Related to Computers with Non-U.S. Versions of Microsoft Programs](# "Click to expand or collapse.")

<div id="ForComputerswithNonUSVersionsofMicrosoftProgramsChild">

> [Special Installation Instructions for Computers with Non-U.S. Versions of Microsoft Windows NT 4.0 and Microsoft Internet Explorer](#nonusnt40)

> [BiDi Systems Must Have Localized Version of Internet Explorer 4.0 SP 1 Before English Visual Studio 6.0 Is Installed](#localizediespneededforenglishvs)

> [NEC PC 98 Installation Issue](#necpc98)

</div>

##### [Data Access SDK 2.0](# "Click to expand or collapse.")

<div id="DASDKChild">

> [Install Requirements](#installreq)

> [How to Install the Microsoft Data Access SDK 2.0](#toinstallmdacsdk2)

> [Before Using SQL Server 6.5 or Older with MDAC 2.0](#sql65orolderwithmdac2)

> [When Microsoft Internet Explorer Setup Installs Older Versions of MDAC Files](#ieinstallsoldmdacfiles)

</div>

##### To get information on general issues affecting the Visual Studio 6.0 suite, and you acquired the suite, go to the [Microsoft® Visual Studio™](readmevs.htm "Jumps to the Visual Studio Readme (readmeVS.htm).") Readme.

##### For information on issues affecting the Enterprise Edition of Visual Studio 6.0, and you acquired this product, go to the [Microsoft® Visual Studio™, Enterprise Edition](readmeve.htm "Jumps to the VS Enterprise Edition Readme (readmeVE.htm).") Readme.

##### For information on the Help system of the Visual Studio suite of products, go to [MSDN™, the Microsoft Developer Network](readmeDN.htm "Jumps to readmeDN.htm") Readme.

* * *

### Installation Instructions for Visual Studio Programs

This section lists installation-related information on programs and files shipped with Visual Studio 6.0.

#### <a name="releaseversionoverbeta">Installing Over Visual Studio Beta, Pre-Release, and Technical Preview Installations</a>

Do not install the final release of Visual Studio 6.0 on computers that have pre-release, technical preview, or beta versions of any Visual Studio product. File copy targets and registration settings have evolved over the development cycle. Installing the final version on computers with a technology preview, pre-release, or other beta version can result in some final components not being installed, while the earlier beta version remain on the system. The outcome could be an unstable product or worse, an unstable system.

Reformat the hard disk and reinstall the operating system before returning a machine used as a beta test platform into the production environment.

#### <a name="sidebysideinstallation">"Side by Side Installation": Installing Multiple Versions of Visual Studio 6.0 Products on the Same Computer</a>

Visual Studio products with the same version and in the same language—Visual C++ and Visual Basic version 6.0 in English, for example—can be installed separately on the same workstation. Such installations are supported by Microsoft. The Visual Studio 6.0 Installation Wizard detects if other versions of the 6.0 product line have been installed on a developer's workstation.

Mixing different language versions, point releases, or product tiers on the same workstation is generally not supported. This means that the installation may fail, one or more of Visual Studio 6.0 products may not work even if the installation succeeds, or in the worst case you may not be able to uninstall any of the products completely.

If the Wizard generates a warning during installation, the safest course of action is to uninstall the Visual Studio 6.0 product before proceeding. The detection scheme checks for the following scenarios:

*   Users **installing different language versions** of the same product. For example, Japanese Visual Basic and English Visual Basic. Installation of certain combinations is supported.

<table cols="2" frame="below" rules="rows" cellspacing="2" cellpadding="5" border="1">

<tbody>

<tr>

<td><font size="2" face="verdana,arial,helvetica">**Product**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Supported Installation**</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Basic</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to two different locations.</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual C++</font></td>

<td><font size="2" face="verdana,arial,helvetica">No side-by-side installation is supported.</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual FoxPro</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to two different locations.</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual InterDev</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to the same location. You must reinstall after uninstalling one version.</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual J++</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to the same location. You must reinstall after uninstalling one version.</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual SourceSafe</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to the same location. You must reinstall after uninstalling one version.

**Note**   The UI language chosen when you run SourceSafe will be based on the system's language settings. If that language is not installed for SourceSafe, it will use English instead.

</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">MSDN</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install to default directory.</font></td>

</tr>

</tbody>

</table>

*   Users **installing different tiers of Visual Studio 6.0 products**. For example, Visual J++ Standard Edition and Visual InterDev Professional Edition. Installing different tiers of the same product on the same workstation is not supported.

*   Users **installing point releases**. Upgrading a later point release of Visual Studio over an earlier point release is supported. However, installing earlier versions over later versions is not supported.

*   Users **installing stand-alone versions of Visual Studio 6.0 products over the versions installed from Visual Studio 6.0 Professional or Enterprise**. For example, Visual FoxPro 6.0 over Visual Studio Professional 6.0\. Installing a stand-alone version of the same language versions (English) of Visual Studio 6.0 products is supported. It is safe to install Visual FoxPro 6.0 (English) from the stand-alone version on a workstation that already has Visual Basic 6.0 installed from Visual Studio Professional Edition.

#### <a name="installingondualbootcomputers">Warning When Installing on Dual-Boot Computers</a>

If you have a dual-boot computer and want to install and run Visual Studio programs with both operating systems, you must install these products into separate directories.

Installing a Visual Studio product, such as Visual C++ or Visual Basic, multiple times on the same directory can result in undefined behavior. Installing a product to the same location from each operating system is sometimes done to save disk space, but it will lead to problems and is not supported.

For example, if you install onto the same directory, you will not be able to fully uninstall the product from both systems. Uninstalling on one system may result in undefined behavior, including the removal of system files from the other system.

#### <a name="installationonsharedcddrive">Installing Visual Studio from a Shared CD Drive</a>

If you are installing Visual Studio 6.0 from a shared compact disc drive, name the share with less than nine characters and with no embedded spaces in the name.

#### <a name="letiefinish">Let Microsoft Internet Explorer Setup Finish Before Proceeding with Visual Studio Installation</a>

During Visual Studio setup, the Installation Wizard will install Internet Explorer 4.01 Service Pack (SP) 1\. Near the end of the Internet Explorer setup, the Internet Explorer setup wizard will restart your computer. The Internet Explorer setup wizard will automatically restart and continue copying updated files and configuring your system.

On some computers, the Visual Studio Installation Wizard may also start while the Internet Explorer setup wizard is finishing this task. You must let the Internet Explorer setup wizard complete its processing before continuing with Visual Studio setup.

Specifically, it is vital that you do not continue with setup to the point of restarting the computer again. Restarting the computer during the final configuration phase of Internet Explorer will corrupt the Visual Studio setup. The Internet Explorer setup wizard shows progress indicators while in its final phase. When these progress indicators disappear, it is safe to proceed with the Visual Studio Installation Wizard.

#### <a name="ieinstallsoldmdacfiles">When Microsoft Internet Explorer Setup Installs Older Versions of MDAC Files</a>

The Microsoft Data Access (MDAC) files installed by Microsoft Internet Explorer 4.0 setup may be older than the MDAC files installed by Visual Studio 6.0 products. If you install Internet Explorer on a computer that already has Visual Studio 6.0, and you get a message asking you to confirm whether you want to install older versions of MDAC files, choose to keep the newer components currently on your computer.

#### <a name="webpublishingwizarddisc">When the Installation Wizard Looks for A Web Publishing Wizard Disc</a>

When installing Visual Studio 6.0 or the Visual J++ Technology Preview 2, if you get a dialog box asking you to insert the Web Publishing Wizard disc, close the dialog box and proceed with the installation.

Neither Visual Studio nor Visual J++ ships a Web Publishing Wizard on a separate disc. Users may get this message when they are installing Visual Studio or Visual J++ on computers that have Temp directories set to removable drives, such as an Iomega Jaz drive.

After your Visual Studio or Visual J++ installation is complete, if you want to install the Web Publishing Wizard, do the following:

1.  Set your Temp environment variable to a directory on fixed media, such as your hard drive.
2.  Run wpie15.exe from _[CD Drive:]_ \setup of the compact disc.
3.  After Web Publishing Wizard setup is complete, reset your Temp environment variable directory to its previous directory, if necessary.

#### <a name="installingclienttoolsafterinstallingvs">Installing Client Tools and Server Components After Visual Studio 6.0 Products Are Installed</a>

The setup procedure is made up of several components. These components are not launched by **Add/Remove Programs** in the **Control Panel**. When you use **Add/Remove Programs**, you will only get to the portion of setup specific to the product installation.

To install any of the following tools, you must run the full setup.

*   Application Performance Explorer
*   Data Access Components 2.0
*   FrontPage 98
*   FrontPage 98 Server Extensions
*   InstallShield
*   NT Option Pack for Windows 95
*   Visual FoxPro Server Examples
*   Visual InterDev Server Components
*   Visual SourceSafe Server
*   Visual Studio Analyzer
*   MSDN

To install any of the listed tools after you have installed any Visual Studio 6.0 products, run setup.exe from compact disc 1\. This action will start the full setup in a "maintenance mode." You will have all of the options you had when you first installed the Visual Studio 6.0 product, but you will not have to go through all of the preliminary dialog boxes.

#### <a name="howtocontacttechnicalsupport">How to Contact Technical Support</a>

The online documentation includes complete information on how to get support and support options, including free support and online support. Click the MSDN Library Visual Studio 6.0 icon and open the Visual Studio Documentation. Support information is in Technical Support, under Getting Started with Visual Studio 6.0.

> **Note**   You must install MSDN to get the online documentation.

You can look up support information on the Web at [http://www.microsoft.com/support](http://www.microsoft.com/support). In addition, you can call (425) 635-7012.

* * *

### <a name="serversidesetups">Installing Server-Side Components</a>

This section lists installation issues identified for server-side components shipped with Visual Studio.

#### <a name="minimumreqsforserversideinstall">Minimum Requirements for Installation and Operation of Server-Side Components</a>

Consult the following table for information on operating system, browser, and other dependency requirements for installation and use of server-side components.

**Table of Minimum Requirements for Installation of Server-Side Components**

<table rules="all" cols="6" frame="below" cellspacing="1" cellpadding="5" border="1">

<tbody>

<tr>

<td><font size="2" face="verdana,arial,helvetica">**Component**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**NT Server**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**NT Workstation**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Windows 95/98**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Requires Microsoft Internet Explorer**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Other Dependencies**</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Windows NT Option Pack 4.0</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Limited on Win95</font></td>

<td></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">SQL Server 6.5 (DEV Edition)</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 3.51 +</font></td>

<td><font size="2" face="verdana,arial,helvetica">Installs some tools on Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">No</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">SQL Server Debugging Service</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Srvr. 3.51 Sp5 or better</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">No</font></td>

<td><font size="2" face="verdana,arial,helvetica">Needs SQL server 6.5 (SP3)</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual SourceSafe Server Components</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Version 4 for viewing HTML Help</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Posting Acceptor (2.0)</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install NTOP before PA 2.0</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Remote Machine Debugging (Script Debugging)</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Version 4 or later</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual InterDev Server Components</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Version 4 or later</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install NTOP, MDAC, FP Extensions before VIDSS</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">FrontPage Server Extensions</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Version 4 or later</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install NTOP, MDAC before FP Extension</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Fox ISAPI Samples and Extensions</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">NO OS dependencies (samples)</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">Any generic browser</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Studio Analyzer</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95 (with DCOM update)</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Only on W95 to get DCOM</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Application Performance Explorer</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0 SP3</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95 (with DCOM update)</font></td>

<td><font size="2" face="verdana,arial,helvetica">Yes. Only on W95 to get DCOM</font></td>

<td><font size="2" face="verdana,arial,helvetica">None</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">MDAC 2.0 Update</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0</font></td>

<td><font size="2" face="verdana,arial,helvetica">Windows 95</font></td>

<td><font size="2" face="verdana,arial,helvetica">No</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install after NTOP and Before SNA</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">SNA server</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT4 Srvr.</font></td>

<td><font size="2" face="verdana,arial,helvetica">NT Workstation 4.0</font></td>

<td><font size="2" face="verdana,arial,helvetica">---</font></td>

<td><font size="2" face="verdana,arial,helvetica">No</font></td>

<td><font size="2" face="verdana,arial,helvetica">Install after MDAC and MTS</font></td>

</tr>

</tbody>

</table>

#### <a name="setupalreadyrunning"></a>"Setup Already Running" Message Shows Up During Installation of Server-Side Components

When you install the Visual Studio 6.0 server-side components on a Windows NT server computer, using the Installation Wizard, you may encounter the message "Another copy of Setup is already running. Complete the other Setup or restart Windows."

This situation typically occurs on slow computers where the Wizard timer runs out while waiting for an ACME setup to finish, and the Wizard starts the next setup.

Click **OK** in the message box. This action will tell the Wizard to terminate one of the conflicting processes and continue with the remaining installations. The summary page that is automatically generated at the end of setup will list the components, if any, that were not completely installed.

To install the specific component that failed, run setup wizard again.

#### <a name="servercomponentsonwin95"></a>Installing Server Components on Windows 95

_It is recommended that you install all server applications on computers running Windows NT._

Enterprise and Professional Editions of Visual Studio 6.0 products are packaged with a variety of Microsoft server applications specifically tailored for the Visual Studio developer. Most applications can be installed on either Windows 95 or Windows NT operating systems. We recommend installing all server applications on Windows NT, either Workstation or Server.

If you choose to set up servers on a Windows 95 computer, the order of installation is important. On Windows 95 some applications must be installed before others for the installation to complete successfully and the product to work. Install the components in the following order:

1.  NT Option Pack
2.  FrontPage 98 Server Extensions
3.  Data Access Components 2.0
4.  Visual InterDev Server Components
5.  Application Performance Explorer
6.  Visual Studio Analyzer

*   (Any Order) Visual SourceSafe Server
*   (Any Order) Visual FoxPro Server Samples

The Installation Wizard presents these options in the same order. Again, ordering is significant on Windows 95 only.

For other issues relating to Windows 95 computers, go to [Issues Specific to Windows 95 Computers](#forwin95)

#### <a name="sqlandwinntop"></a>Known Compatibility Issues with SQL Server 6.5 and Windows NT Option Pack 4.0

If you install SQL Server 6.5 on a computer with Windows NT Option Pack 4.0 installed, some of your Design Time Controls (DTCs) may be overwritten.

If this happens, you will get an error message when you launch Microsoft Transaction Server (MTS). The message will instruct you to reinstall MTS.

To prevent this situation, install NT Option Pack after you install SQL Server.

* * *

### <a name="configuringdebugging">Configuring for Debugging</a>

Information in this section addresses issues on debugging and configuring computers for debugging services.

#### <a name="iispatchforaspdebugging">For ASP Debugging, Install IIS Patch After Installing BackOffice</a>

Internet Information Server (IIS) has a patch that fixes problems related to debugging Active Server Pages (ASP) from Visual InterDev. This patch also fixes a Windows 95/98 problem in which changes to the Global.asa would not be reflected in your application (such as adding, changing, or removing data connections) until you stopped and restarted your Web server.

To ensure that ASP debugging works properly, or to address the Windows 95/98 issue, apply the patch after the BackOffice Installation Wizard has finished.

**To apply the IIS patch on Windows NT computers**

1.  Run \IIS\WinNT\ASP2FIX1.exe from the installation disc.

<table rules="all" frame="below" cellspacing="1" cellpadding="5" border="1">

<tbody>

<tr>

<td><font size="2" face="verdana,arial,helvetica">**Product**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Disc Location**</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Studio, Professional Edition</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#2</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Studio, Enterprise Edition</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#3</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual InterDev</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#1</font></td>

</tr>

</tbody>

</table>

3.  Restart when prompted.

**To apply the IIS patch on Windows 9_x_ computers**

1.  Stop the Web server from the **Command Prompt**: Type **pws/stop** and press ENTER.

3.  In the \_<windows>_\system\inetsrv directory, rename Asp.dll to Asp.old

5.  From the \IIS\Win9_x_\ directory of the installation disc, copy Asp.dll and paste it to the \_<windows>_\system\inetsrv directory on your computer.

<table rules="all" frame="below" cellspacing="1" cellpadding="5" border="1">

<tbody>

<tr>

<td><font size="2" face="verdana,arial,helvetica">**Product**</font></td>

<td><font size="2" face="verdana,arial,helvetica">**Disc Location**</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Studio, Professional Edition</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#2</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual Studio, Enterprise Edition</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#3</font></td>

</tr>

<tr>

<td><font size="2" face="verdana,arial,helvetica">Visual InterDev</font></td>

<td><font size="2" face="verdana,arial,helvetica">CD#1</font></td>

</tr>

</tbody>

</table>

8.  Return to the **Command Prompt** and restart the Web server: Type **pws/start** and press ENTER.

#### <a name="sqldebuggingoncomputerswithsql65andvc5orhigher">Using SQL Debugging Services on a Computer with SQL Server 6.5 and Visual C++ 5.0 or Higher Installed</a>

To use SQL Debugging services on a computer that has SQL Server 6.5 and Visual C++ 5.0 or higher installed, make sure that the Remote Automation (RA) configuration properties of the computer are set correctly.

**To check RA configuration properties**

1.  Run dcomcnfg.exe.
2.  Select Remote Automation CLSID_StubMarhsaler.
3.  Click **Properties**.
4.  In the **Identity** tab, select Interactive User.

Also, your SQL Debugging scenarios may not work if you run SQL Server as a service under the Local System account. You must select **This Account** and enter a valid account and password.

* * *

### <a name="forwin95">Issues Specific to Windows 9_x_ Computers</a>

This section lists issues identified when Visual Studio 6.0 is installed on Windows 95 or Windows 98 computers.

#### <a name="windows95registrysize">Windows 95 Registry Size: 64 KB Limitation May Cause A Warning During Visual Studio Installation</a>

A 64-KB limitation in the size of the SharedDLL key in the Windows 95 system registry may generate a warning that appears when you install Visual Studio 6.0.

Before continuing with setup, you should shorten the install path where you plan to install Visual Studio 6.0, reducing the amount of registry space required.

Additionally, you can uninstall programs you no longer use by utilizing the Add/Remove Programs from the Control Panel. The registry keys used exclusively by those programs will then be deleted.

To save further on registry space used by programs you intend to keep, uninstall, then reinstall these programs to shorter installation paths.

Consider using the RegClean utility, designed to clean up unnecessary entries in your registry. For more information and a download link, go to [http://support.microsoft.com/support/kb/articles/q147/7/69.asp](http://support.microsoft.com/support/kb/articles/q147/7/69.asp)

**Note**   On Windows NT Workstations and Servers, Visual Studio setup will automatically resize the registry.

#### <a name="whenautologonisenabled">Disable Autologon Before Running Visual Studio 6.0 Setup</a>

Visual Studio setup may fail on Windows 95 computers configured with Autologon.

Before you install Visual Studio 6.0 or any of its products on a Windows 95 computer with Autologon enabled, turn off Autologon by following the instructions found at [http://support.microsoft.com/support/kb/articles/q141/8/58.asp](http://support.microsoft.com/support/kb/articles/q141/8/58.asp).

> **Note**   This article contains several additional steps that may not be relevant on your system.

If you installed Visual Studio products on a Windows 95 computer configured with Autologon, and setup failed, repeat your setup steps with Autologon disabled.

#### <a name="internetconnectiondialog">An Internet Connection Dialog Box May Appear at Startup of Windows or Other Applications</a>

If remote connections are enabled in Windows 95 or Windows 98, the system may try to initiate an Internet connection at Windows startup or at the start of many applications. This behavior is sometimes called "autodial" or "autoconnect." You can turn off this behavior by setting the registry key EnableRemoteConnect to "N."

To do this, create a text file "DisbleAutoConnect.reg" with exactly the following three lines:

> REGEDIT4

> [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\OLE]

> "EnableRemoteConnect"="N"

Changing this setting to disable remote connections should not prevent any of your normal Internet activities, and this setting is the default for most systems. However, enabling remote connections is necessary for some features of DCOM (see [http://support.microsoft.com/support/kb/articles/Q177/3/94.asp](http://support.microsoft.com/support/kb/articles/Q177/3/94.asp)).

If there are instances when you need to have remote connections enabled, create a second REG file, "EnableRemoteConnect.reg", with exactly the following 3 lines:

> REGEDIT4

> [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\OLE]

> "EnableRemoteConnect"="Y"

Run "EnableAutoConnect.reg" to make the setting, and then run "DisbleAutoConnect.reg" to disable it when autoconnect is no longer needed.

#### <a name="resumingsetupafterinstallingpws">Installation Wizard May Not Restart After PWS Is Installed on Windows 95 Computers</a>

If you choose to install Personal Web Server (PWS) on a Windows 95 computer, the Installation Wizard may not resume correctly after the computer restarts. To proceed, start Setup.exe again from the first disc of your Visual Studio 6.0 CD set. The Installation Wizard automatically resumes setup at the correct point.

#### <a name="frontpage98onwin95">Installing Microsoft FrontPage 98 Extensions on Some Windows 95 Computers</a>

When the Installation Wizard launches other client or server setups, the Wizard becomes invisible and waits until the component installation is complete. The Wizard then reappears, enabling the user to install another component.

When you install Microsoft FrontPage 98 extensions on some Windows 95 computers, the Installation Wizard may remain hidden for several minutes after the FrontPage setup is complete.

While the Wizard is hidden, you cannot launch the setup program again. A second Installation Wizard will not start when the program detects that one is already running.

* * *

### <a name="vs6andothers">Notes Impacting Other Installed Programs</a>

This section lists installation issues that may affect programs already installed on your computer.

#### <a name="iisamexchangedriver">IISAM Exchange Driver Will Fail if Microsoft Exchange or Microsoft Outlook Is Not Already Installed</a>

The IISAM Exchange driver requires that Microsoft Exchange or Microsoft Outlook be fully installed on your computer prior to installation of Visual Studio. If neither is installed, the IISAM Exchange driver will not be self-registered.

To correct the problem after you've installed Visual Studio 6.0, you can install Microsoft Exchange or Microsoft Outlook and then manually self-register the IISAM Exchange driver using this command line:

<font size="2" face="Courier">Regsrv32 msexch35.dll</font>

* * *

### <a name="fornonusversions">Issues Related to Computers with Non-U.S. Versions of Microsoft Programs</a>

This section lists known setup issues related to computers with non-U.S. versions of Microsoft programs.

#### <a name="nonusnt40">Special Installation Instructions for Computers with Non-U.S. Versions of Microsoft Windows NT 4.0 and Microsoft Internet Explorer</a>

If you are installing this version of Visual Studio 6.0 on a non-U.S. version of Windows NT 4.0, you must first install the appropriate language version of Windows NT 4.0 Service Pack 3.

To install this version of Visual Studio 6.0 on a computer that uses an international version of Microsoft Internet Explorer, you must install the appropriate language version of Microsoft Internet Explorer.

The international versions of Windows NT 4.0 Service Pack 3 are available from these locations:

*   [ftp://ftp.microsoft.com/bussys/winnt/winnt-public/fixes](ftp://ftp.microsoft.com/bussys/winnt/winnt-public/fixes)*   [http://www.microsoft.com/support/winnt/intlsp.asp](http://www.microsoft.com/support/winnt/intlsp.asp)

The international versions of Microsoft Internet Explorer 4._x_ are available from:

*   [http://www.microsoft.com/ie/download/](http://www.microsoft.com/ie/download/)

#### <a name="localizediespneededforenglishvs">BiDi Systems Must Have Localized Version of Internet Explorer 4.0 SP 1 Before English Visual Studio 6.0 Is Installed</a>

Before installing the English version of Visual Studio 6.0 on a system that is configured with a bidirectional (BiDi) character set, such as Hebrew or Arabic, you first must install the localized version of Microsoft Internet Explorer 4.01 Service Pack 1.

The international versions of Microsoft Internet Explorer 4.x are available from:

*   [http://www.microsoft.com/ie/download/](http://www.microsoft.com/ie/download/)

#### <a name="necpc98">NEC PC 98 Installation Issue</a>

On NEC PC98's where the C drive is a floppy disk, if you get the error _Cannot read drive \Device\Floppy0:_, place a formatted floppy disk in the drive. Make sure that the drive door is closed and that the disk is properly formatted. Then, proceed with installation.

* * *

### <a name="dasdkissues">Data Access SDK 2.0</a>

This section discusses all issues identified in Data Access SDK 2.0.

#### <a name="installreq">Install Requirements</a>

The Data Access SDK delivered with Visual Studio requires that the Microsoft Data Access components be installed prior to installing this SDK. Otherwise, when the SDK setup is run, you will get the message:

> ODBC is not installed on this machine. If you continue, you will receive errors. Do you wish to continue anyway?

To resolve this, make sure that you have run the Visual Studio setup before installing the Data Access SDK.

#### <a name="toinstallmdacsdk2">How to Install the Microsoft Data Access SDK 2.0</a>

The Microsoft Data Access SDK 2.0 can be installed by running the file DASDK.exe from the \dasdk directory on disc 2.

The SDK includes Microsoft Data Access Components samples, and further information and tools for ODBC and OLE DB developers.

#### <a name="sql65orolderwithmdac2">Before Using SQL Server 6.5 or Older with MDAC 2.0</a>

You must update the catalog procedures if you plan to use SQL Server 6.5 or older with MDAC 2.0\. See the SQL Server Driver Help file, drvssrvr.hlp, for more information.

Typically, you will find drvssrvr.hlp

*   On NT systems: \winnt\system32
*   On Windows 95: \windows\system

</font>