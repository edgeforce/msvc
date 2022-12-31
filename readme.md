<!----------------------------------------------------------------------------->
<!--                            BEGIN JSCRIPT                                -->
<!--                                                                         -->
<script language="JSCRIPT">

  function checkExpand( )
  {
     if ("" != event.srcElement.id)
     {
        var ch = event.srcElement.id + "Child";
        var el = document.all[ch];
        if (null != el)
        {
           el.style.display = "none" == el.style.display ? "" : "none";
           if (el.style.display != "none")
           //   el.scrollIntoView(true);
           event.returnValue=false;
        }
     }
  }
</script>
<!--                                                                         -->
<!--                             END JSCRIPT                                 -->
<!----------------------------------------------------------------------------->

<!----------------------------------------------------------------------------->
<!--                             BEGIN README                                -->
<!--                                                                         -->
<!--                     Visual C++ Readme Version 6.0                       -->
## <a name="readmevc_top">Visual C++ Readme</a>

<sup>©</sup>1998 Microsoft Corporation. All rights reserved.

Other product and company names herein may be the trademarks of their respective owners.

_Visual C++<sup>®</sup> 6.0 Readme_ includes updated information for the documentation provided with Microsoft<sup>®</sup> Visual Studio<sup>®</sup> 6.0 Development System for Windows<sup>®</sup> and the Internet. The information in this document is more up-to-date than the information in the Help system. Many of the issues outlined in this document will be corrected in upcoming releases.

For _general installation issues_ on the Visual Studio 6.0 suite of products, including side by side product installation, see the [Installation Notes](install.htm "Jumps to the installation readme (install.htm).") Readme (install.htm).

For other issues on the Help system of the Visual Studio suite of products, go to [MSDN™, the Microsoft Developer Network Readme.](readmeDN.htm "Jumps to MSDN Readme")

Contents <font size="2" face="Verdana,Arial,Helvetica" color="#000000">- Click any of the items below</font> to expand:

##### [Setup Issues](# "Click to collapse or expand")

<div id="SetupChild">

> [Protected-Mode CD-ROM Driver Required on Windows 95 for Visual C++ Installation](#Setup_3)

> [Use Knowledge Base Articles to Solve Setup and Operating Problems](#Setup_4)

> [How to Report Visual C++ Bugs on the WWW](#Setup_5)

> [Viewing "ANSI Character Code Chart" in HTML Help Requires an English System](#Setup_6)

> [Resource Viewer and Compiler Not Installed in Some Custom Setup Configurations](#Setup_7)

> [Avoiding Problems Associated with Installing New SDKs](#Setup_8)

</div>

##### [Build Issues](# "Click to collapse or expand")

<div id="BuildingChild">

> [Help File Names with European Characters Do Not Copy Correctly on Windows 95](#Build_5)

> ["Update All Dependencies" Menu Item Removed](#Build_6)

</div>

##### [Documentation Issues](# "Click to collapse or expand")

<div id="DocumentationChild">

> [New Help Viewer](#Doc_1.1)

> [Sample Code Sometimes Does Not Cut and Paste Properly](#Doc_1.2)

> [CToolbar::SetButtonStyles Documentation Missing Information](#Doc_6)

> [Error in Topic "Enabling STRICT Type Checking"](#Doc_7)

> [Error in Topic "Modifying IntelliSense Options"](#Doc_8)

> [Error in Topic "Create a Utility Project"](#Doc_8.1)

> [Developing Context-Sensitive Help Using HTML Help](#Doc_9)

> [Error in Topic "Receiving HTML Help Notification Messages in an MFC Application"](#Doc_11)

> [Addendum to AutoClik Tutorial Topics](#Doc_12)

> [Tree View Controls Not Documented](#Doc_13)

> [References to MFC Version 4.22 in the Documentation](#Doc_15)

> [wmemchr, wmemmove, wmemcpy, wmemset Not Available from C](#Doc_17)

> [Undocumented CTabCtrl Styles](#Doc_18)

> [CControlBar::GetDockingFrame Documentation Does Not State Return Value When Control Bar Is Floating](#Doc_19)

> [Addendum to DECLARE_CLASSFACTORY_AUTO_THREAD Topic](#Doc_20)

> [Error in "CComModule::Init" Topic](#Doc_21)

> [Errors in "Implementing a Simple Consumer" Topic](#Doc_23)

> [Addendum to CProgressCtrl Topic](#Doc_24)

> [Error in "Implementing a Window with CWindowImpl" Topic](#Doc_25)

> [Errors in CDC::Escape Topic](#Doc_26)

> [ATLCOLUMNINFO Structure Not Documented](#Doc_27)

> [ATLTRACE and AtlTrace Documentation Incorrectly Refer to Dump Device](#Doc_28)

> [Errors in "How Do I Reference a Property in My Provider?" Topic](#Doc_29)

> [Undocumented Function AfxDebugBreak](#Doc_31)

> [Undocumented ATL Consumer Method CDataSource::OpenWithServiceComponents](#Doc_32)

> [Errors in AddProject Method Topic](#Doc_33)

> [Addendum to Documentation for Microsoft UpDown Control](#Doc_34)

> [Errors in "IDispatchImpl" and "IProvideClassInfo2Impl" Topics](#Doc_30)

> [CFileDialog Undocumented Functions](#Doc_10)

</div>

##### [ActiveX Control Issues](# "Click to collapse or expand")

<div id="ActiveXChild">

> [New ActiveX Control Test Container Cannot Open Saved Sessions Files Created by Previous Version](#ActiveX_Control_Issues_1)

> [Problems Accessing ActiveX Control Test Container Help](#ActiveX_Control_Issues_2)

> [Some ActiveX Controls Created with Visual Basic Generate Error in Test Container on Resize](#ActiveX_Control_Issues_4)

> [Oracle Joins and MSRDC20.ocx (Remote Data Control V2)](#ActiveX_Control_Issues_5)

> [Current, Localized ActiveX Redistributable Components](#ActiveX_Control_Issues_6)

</div>

##### [Language Issues](# "Click to collapse or expand")

<div id="LanguageChild">

> [Size Mismatch for Type bool in Visual C++ 4.2 Programs Built with Visual C++ 6.0](#Language_Issues_3)

> [Support for Member Templates](#Language_Issues_4)

</div>

##### [Libraries Issues](# "Click to collapse or expand")

<div id="LibrariesChild">

> [Using MFC with New SDK Releases](#MFC_1)

> [Incomplete Documentation for CWnd::RepositionBars](#MFC_3)

> [Incorrect Example Code in the CArchive::MapObject Member Function](#MFC_5)

> [Some ATL Object Stock Properties Must Be Initialized Before Use in Visual Basic 5.0 Containers](#MFC_5.1)

> [ATL Font and Picture Properties May Require Changes to the IDL File](#MFC_5.3)

> [Documentation Missing for MFC Message Map Macro ON_WM_SETTINGCHANGE](#MFC_6)

> [TN024 Doesn't Identify All Custom MFC Resource Types](#MFC_7)

> [MFC DAO Classes Will Work with Either DAO 3.0 or DAO 3.5](#MFC_8)

> [Using DAO with a Secure Database](#MFC_9)

> [MFC Loads Wrong Resource in Extension .dll](#MFC_13)

> [Call _findclose After Using _findfirst or _findnext](#MFC_14)

> [Format Specification Not Supported in COleDateTime and COleDateTimeSpan Classes](#MFC_20)

> [IsBadHugeReadPtr, IsBadHugeWritePtr, IsBadStringPtr, IsBadWritePtr, and Access Violations](#MFC_21)

> [ServerSupportFunction No Longer Supports SF_REQ_GET_CONNID](#MFC_23)

[](#MFC_23)

> [](#MFC_23)[Hot Track Property for Spin Control Not Implemented](#MFC_24)

[](#MFC_24)

> [](#MFC_24)[COleDateTime::GetStatus Returns Valid for Default Constructor](#MFC_25)

[](#MFC_25)

> [](#MFC_25)[Opening a DLL as "Resources" Might Require Installation of .nls Files](#MFC_26)

[](#MFC_26)

> [](#MFC_26)[Multiple Language Resource Files](#MFC_27)

[](#MFC_27)

> [](#MFC_27)[AfxDumpStack API Will Not Work until NT 5.0 Beta 2](#MFC_28)

[](#MFC_28)

> [](#MFC_28)[Changes to IObjectSafetyImpl](#MFC_29)

> [Some Concrete MFC Classes Have No vtable When Built, Causing GPF on Deletion](#MFC_30)

> [ATLCOLUMNINFO Structure Not Documented](#Doc_27)

> [Errors in "IDispatchImpl" and "IProvideClassInfo2Impl" Topics](#Doc_30)

> [CFileDialog Undocumented Functions](#Doc_10)

</div>

##### [Wizard and Other User-Interface Issues](# "Click to collapse or expand")

<div id="WizardChild">

> [Using the MTS Option in ATL COM AppWizard](#Wizards_2)

> [Save .idl File Before Invoking ATL Add Method or ATL Add Property](#Wizards_2.15)

> [Databinding Dialog Controls in an OLE DB Application](#Wizards_2.16)

> [MFC AppWizard Generated Code Needs Editing for Tables and Providers with Spaces in Names](#Wizards_2.18)

> [Two New Template Variables Available to Custom AppWizards](#Wizards_6)

> [Problems with ClassWizard Generated Wrapper Classes for Visual Basic 5.0 ActiveX Servers](#Wizards_7)

> [ATL Controls in Visual Basic 5.0 Containers](#Wizards_8)

> [ClassView's Add Method and Add Property Dialog Boxes Sometimes Allow Illegal Return Types for Custom Interfaces](#Wizards_10)

> [MFC Header stdafx.h May Not Have All Necessary #include's from a Visual Modeler Code Generation](#Wizards_11)

> [IntelliSense Does Not Display Class Members for Inline Member Functions](#Wizards_13)

> [IntelliSense Might Present Outdated Information with Operating Systems That Ship After Visual C++ 6.0](#Wizards_14)

> [IntelliSense Limitations](#Wizards_15)

> [ClassView's Implement Connection Point: Problem with DIIDs in the Connection Point Map](#Wizards_16)

> [Help for All Tab in ActiveX Controls Properties Sheet Not Available](#Wizards_17)

> [Notes for MMC Snapin Object in ATL Object Wizard](#Wizards_18)

> [ATL Control's HWND Stock Property Causes Error Dialog in VB](#Wizards_19)

> [Program Does Not Compile When You Insert a New ATL Object into an MFC Database Application Using OLE DB Datasource](#Wizards_20)

> [Warning on ATL Object Wizard's "Free Threaded Marshaler" Option](#Wizards_21)

> [Project Names with Upper-ASCII or DBCS Characters Cause Build Errors in Custom AppWizard-Generated Projects](#Wizards_22)

> [Assertion in AppWizard-Generated MDI Active Document Container](#Wizards_23)

</div>

##### [Microsoft Transaction Server Issues](# "Click to collapse or expand")

<div id="MTSChild">

> [Read Microsoft Transaction Server (MTS) Readme](#MTS_1)

> [MTS Objects Created with the ATL AppWizard Require Manual Running MTXRereg.Exe](#MTS_2)

> [Disable Transaction Time Out While Debugging](#MTS_3)

> [No Proxy/Stubs with Dual Interfaces](#MTS_4)

> [Older Versions of MSDTC May Cause MTS Transaction Failures](#MTS_5)

</div>

##### [Microsoft Visual Database Tools Issues](# "Click to collapse or expand")

<div id="DataToolsChild">

> [DataView "Create New Extended Stored Procedure" Dialog Box Truncates Path of DLL Name](#Data_Tools_2)

> [Visual C++ 6.0 Professional Edition Includes Read-Only Microsoft Database Tools](#Data_Tools_3)

> [Jet Versions Supported by Visual C++](#Data_Tools_4)

</div>

##### [Sample Program Issues](# "Click to collapse or expand")

<div id="SamplesChild">

> [Ignore SFL Directory in Samples](#Sample_Program_Issues_3)

> [MINIMAL Sample Needs Modification to Build](#Sample_Program_Issues_16)

> [COMMAP: Remove Mktyplib Compat Mode for MIDL](#Sample_Program_Issues_18)

> [AtlTangram: Needs Additional Files in Include Path](#Sample_Program_Issues_20)

> [Some Samples Have Source Safe Linkage](#Sample_Program_Issues_21)

> [DBVList](#Sample_Program_Issues_22)

> [ComplexDB](#Sample_Program_Issues_24)

> [ATLMTO Sample Needs to Have ATL_MIN_CRT Turned Off](#Sample_Program_Issues_25)

> [Addendum to ComplexDB Sample Abstract](#Sample_Program_Issues_26)

> [ACCSPICT Sample Command Line Error](#Sample_Program_Issues_27)

> [CIRC and STOCKTICKERATL Samples Get MIDL Error](#Sample_Program_Issues_28)

> [CIRCPROPS Sample Cannot Open circ.h Because of CIRC Problem](#Sample_Program_Issues_29)

> [AUTODRIVE Gets Command Line Error](#Sample_Program_Issues_30)

> [Ignore SourceSafe Dialog When Loading ActiveDoc and Polygon ATL Samples](#Sample_Program_Issues_31)

> [Rebuild All on SDK's INOLE2 Samples Will Give Linker Error](#Sample_Program_Issues_32)

> [Workspace Files for the VCCOM COMMAP Sample Have Mismatched Targets](#Sample_Program_Issues_33)

> [Known Problems in MYPROV Sample](#Sample_Program_Issues_34)

> [ActiveDoc ATL Sample Defaults to Unicode](#Sample_Program_Issues_35)

</div>

##### [OLE DB Issues](# "Click to collapse or expand")

<div id="OLEDBChild">

> [OLE DB Consumer Template Samples](#OLE_DB_2.1)

> [OLE DB Provider Templates Sample](#OLE_DB_2.2)

> [Remove UUID2.lib from Link Line of OLE DB SDK TableCopy Sample](#OLE_DB_4)

> [TableCopy Faults with Oracle Data Connections](#OLE_DB_5)

> [Configuring OLE_DB_xx Data Sources in the ODBC Administrator](#OLE_DB_6)

> [Binding Multiple Complex Databound Controls to the Same ADO Data Source Will Crash Application on Exit](#OLE_DB_9)

> [Some Controls Do Not Draw Correctly in the Resource Editor](#OLE_DB_10)

> [Binding ADODC to Controls then Editing Record Source Will Draw Spurious Errors](#OLE_DB_11)

> [Hierarchical Flex Grid Does Not Refresh on Second Query](#OLE_DB_12)

> [Porting Providers Created with Visual C++ Technology Preview Release to Version 6.0](#OLE_DB_14.1)

> [Porting Consumers Created with Visual C++ Technology Preview Release to Version 6.0](#OLE_DB_14.2)

> [Cannot Use ADO Databound Controls with Remote Data Source Control (MSRDC), or RDO Databound Controls with ADO Data Source Control (ADODC)](#OLE_DB_15)

> [Known OLE DB Provider Problems with Visual C++ Wizards](#OLE_DB_16)

> [Notes on Running OLE DB Provider Conformance Tests](#OLE_DB_17)

> [Simple Bound ADO Databound Controls Must Be Associated with a Column](#OLE_DB_18)

> [Some OLE DB Providers Do Not Support Table Names with Spaces](#OLE_DB_19)

> [Databinding Dialog Controls in an OLE DB Application](#Wizards_2.16)

> [MFC AppWizard Generated Code Needs Editing for Tables and Providers with Spaces in Names](#Wizards_2.18)

</div>

##### [SQL and SQL Debugging Issues](# "Click to collapse or expand")

<div id="SQLChild">

> [DataView and IDE Crashes When Opening Table Against DSN Using Oracle's ODBC Driver](#SQL_1)

> [Previous Versions of Visual C++ Cannot Read SQL Diagrams Opened by Later Versions](#SQL_2)

> [Enabling SQL Debugging](#SQL_3)

> [Server-Side Setup Must Check SQL Server Account](#SQL_4)

> [SQL Server OLE DB Provider Requires New instcat.sql](#SQL_5)

> [MultiRead Provider Sample Needs Modification to Run](#SQL_6)

> [SQL Server OLE DB Provider Requires Indexes to be Set on Tables for IRowsetScroll](#SQL_7)

</div>

##### [Compiler, Linker, Debugger, and MIDL Compiler Issues](# "Click to collapse or expand")

<div id="CompilerChild">

> [New Debugger Features](#Compiler_30)

> [Some Linker Options Disable Edit and Continue](#Compiler_37)

> [Use New -opt:win98 Linker Switch If Targeting Windows 98 Platforms](#Compiler_38)

> [Problem with Debugging COM/ActiveX Controls Through Internet Explorer 4.0 or Later](#Compiler_39)

> [STRICT Type Checking Is Enabled by Default](#Compiler_40)

> [Remote Debugging: Debug Monitor Password Field in MSVCMON.exe Disabled](#Compiler_31)

> [_com_error Constructor Changed](#Compiler_34)

> [Breakpoints Set in Some Circumstances Might Not Work](#Compiler_32)

> [Duplicate GUIDs Cause Build Failures Using uuid.lib](#Compiler_35)

> [Using Windbg with Visual C++ 6.0 Projects](#Compiler_1)

> [_ATL_MIN_CRT and Link Error "unresolved external symbol _main"](#Compiler_2)

> [DCOM95 Available for Distributed Applications](#Compiler_3)

> [Debugging Windows API Functions with NT Symbols Loaded](#Compiler_11)

> [If Screen Flashes During Build or the Wrong Code Page Is Used When Debugging a Console Application](#Compiler_12)

> [MIDL2020: error generating type library: save all changes failed](#Compiler_15)

> [Error Command Line Warning MIDL1009:unknown argument ignored](#Compiler_17)

> [/Zn Option Obsolete](#Compiler_41)

> [Delay Loading DLLs or Loading DLLs "on Demand"](#Compiler_42)

> [NT System Symbol Setup Installs Debugging Files Only for the Language of Your Product](#Compiler_43)

> [New Dumpbin Option /LOADCONFIG](#Compiler_44)

> [New Compiler Switch /QIfist](#Compiler_45)

> [Cannot Debug Fibers on Windows 98](#Compiler_46)

> [#pragma data_seg Affects Initialized Data Only](#Compiler_47)

> [Setting Breakpoints and Using Set Next Statement in Edited Code](#Compiler_48)

> [Using the /GX Option (Synchronous Exception Handling) with Command-Line Tools](#Compiler_49)

> [No F1 Help on TCP/IP Network Settings Dialog Box](#Compiler_50)

> [Visual C++ 5.0 Can Read Version 6.0 Projects, but Behavior Is Undefined](#Compiler_51)

> [Windows NT Symbols Setup Gives Erroneous Message](#Compiler_52)

> [AfxDumpStack Does Not Dump Readable Symbols from an MFC Application](#Compiler_53)

> [Browsing Symbol Information Might Cause Access Violation in Projects where excel8.olb Has Been #imported](#Compiler_54)

</div>

##### [Visual SourceSafe Issues](# "Click to collapse or expand")

<div id="VSSChild">

> [Converting a Visual C++ 4.x Project Directly from Source Control](#VSS_1)

> [Using Visual SourceSafe 5.0 with Keyword Expansion Requires Visual Studio 97 Service Pack 1](#VSS_2)

</div>

##### [Visual Component Manager Issues](# "Click to collapse or expand")

<div id="VCMChild">

> ["Related Files Tab (Component Properties Dialog Box)" Topic Incorrect](#RelatedFilesTab)

> [Removing Repository 1.0 Registry Keys](#RemovingRepository10RegistryKeys)

> [Adding Repository Tables to an Existing .mdb File](#AddingrepositorytablestoanexistingMDBfile)

</div>

### <a name="Setup_0"></a>Setup Issues

#### <a name="Setup_3">**Protected-Mode CD-ROM Driver Required on Windows 95 for Visual C++ Installation**</a>

To install Visual C++ 6.0 on Windows 95, you must be running a protected-mode CD-ROM driver. You can verify this by checking the Device Manager. If you are currently using a real-mode CD-ROM driver, contact your CD-ROM drive manufacturer for an updated driver for Windows 95 before installing Visual C++ 6.0.

#### <a name="Setup_4">**Use Knowledge Base Articles to Solve Setup and Operating Problems**</a>

You can use the Knowledge Base articles in the MSDN documentation to resolve known installation and operating problems. Select the **Search** command from the **Help** menu and search for error message or related keywords to find a problem description and resolution.

Knowledge Base articles, written by Microsoft Technical Support Engineers, are also available by connecting to [http://www.microsoft.com/support/](http://www.microsoft.com/support/), then click "support online." You will have to register the first time. After you have registered, enter your email name and password. Choose "Visual C++" in the **Choose a product** drop-down list. Enter the article title or number in the **My question is** text box, then click **Find**.

#### <a name="Setup_5">**How to Report Visual C++ Bugs on the WWW**</a>

Go to [http://www.microsoft.com/regwiz/regwiz.asp](http://www.microsoft.com/regwiz/regwiz.asp) and select "Report a bug in a product." Follow the instructions from there.

#### <a name="Setup_6">Viewing "ANSI Character Code Chart" in HTML Help Requires an English System</a>

The character codes displayed in the "ANSI Character Code Chart" topic will only display correctly if viewed on English systems using an "ANSI-compatible" code page.

#### <a name="Setup_7">Resource Viewer and Compiler Not Installed in Some Custom Setup Configurations</a>

If you install Visual C++ using a custom setup, and omit the Visual C++ resource viewer and compiler, you will not be able to view the project resources.

The workaround is to install Visual C++ with all options (including run-time libraries, MFC and templates, build tools, etc.).

#### <a name="Setup_8">Avoiding Problems Associated with Installing New SDKs</a>

When installing Microsoft SDKs, compare the header and library dates in the SDK files with the files that were shipped with Visual C++. If the SDK files are newer, you should place the SDK directories before the default Visual C++ INCLUDE and LIB directories listed in the Directories tab of the Options dialog in the Tools menu.

### <a name="Build_0"></a>Build Issues

#### <a name="Build_5"></a>Help File Names with European Characters Do Not Copy Correctly on Windows 95

The Help compiler converts the name of the Help file into uppercase characters. On Windows 95, this causes problems when the Visual Studio Build System tries to copy a name that contains European characters (such as umlauted characters) to the output directory for the rest of the project build. This is not a problem on Windows NT.

##### Workaround

Add a copy step with the name of the Help file, in uppercase, to the custom build rule on the .hpj file in the project.

#### <a name="Build_6"></a>"Update All Dependencies" Menu Item Removed

The **Update All Dependencies** item has been removed from the **Build** menu because dependencies are automatically updated in each build. Dependencies are updated at the beginning of the initial build and at the end of every build.

### <a name="Doc_0"></a>Documentation Issues

#### <a name="Doc_1.1"></a>New Help Viewer

Online documentation is now accessed with a Help viewer based on HTML Help. The Help Viewer can either be installed during the Visual Studio installation or from the MSDN CD-ROM. See the [Microsoft Developer Network Library Readme](ReadmeDN.htm) for full details on MSDN installation.

Access the Help Viewer by selecting items on the **Help** menu in the Visual C++ environment. When you bring up Help, you will get a separate window that displays navigation buttons, tabs with contents, index and search, and a pane with text. It is displayed in a similar manner to WinHelp in the Office products. This is the behavior for all Developer Tools products in Visual Studio 6.0.

#### <a name="Doc_1.2"></a>Sample Code Sometimes Does Not Cut and Paste Properly

Line breaks and formatting information may not copy correctly when you copy and paste sample code from the MSDN Library Visual Studio documentation to your code editor. See the item "Sample Code Sometimes Does Not Cut and Paste Properly" in the [MSDN Readme](ReadmeDN.htm) or the [Visual Studio Readme](ReadmeVS.htm).

#### <a name="Doc_6"></a>CToolbar::SetButtonStyles Documentation Missing Information

**CToolbar::SetButtonStyles** is missing the following three style descriptions:

*   **TBBS_AUTOSIZE** - The button's width will be calculated based on the text of the button, not the size of the image.
*   **TBBS_NOPREFIX** - The button text will not have an accelerator prefix associated with it.
*   **TBBS_DROPDOWN** - Creates a drop-down list button. Drop-down buttons send the **TBN_DROPDOWN** notification. If the toolbar has the **TBSTYLE_EX_DRAWDDARROWS** extended style, drop-down buttons will have a drop-down arrow displayed next to them.

#### <a name="Doc_7"></a>Error in Topic "Enabling STRICT Type Checking"

The topic "Enabling STRICT Type Checking" in the _Visual C++ Programmer's Guide_ incorrectly states that STRICT type checking is not defined by default, and that you must explicitly enable it. STRICT type checking is enabled by default as described in [this item](#Compiler_40).

#### <a name="Doc_8"></a>Error in Topic "Modifying IntelliSense Options"

In the topic "Modifying IntelliSense Options," under the heading "To change default key mappings for Intellisense options," Step 3 should have **All commands** instead of **Commands**.

#### <a name="Doc_8.1"></a>Error in Topic "Create a Utility Project"

In the topic "Create a Utility Project" in the _Visual C++ Programmer's Guide_, the instruction in Step 2 to "double-click the Dynamic Link-Library icon" should read "double-click the Utility Project icon."

#### <a name="Doc_9"></a>Developing Context-Sensitive Help Using HTML Help

If you are developing context-sensitive help for your programs and want to use HTML Help rather than WinHelp, read "Help Topics (HTML Help): Context-Sensitive Help for Your Programs" in the _Visual C++ Programmer's Guide_.

Note that there is an error in the topic ["Receiving HTML Help Notification Messages in an MFC Application"](#Doc_11), described below.

#### <a name="Doc_11"></a>Error in Topic "Receiving HTML Help Notification Messages in an MFC Application"

Step 3 of the topic "Receiving HTML Help Notification Messages in an MFC Application" is incorrect. The entire topic should read as follows:

To receive notification messages from HTML Help within an MFC program, you must:

1.  Define a symbol in your Visual C++ project. This example uses a symbol called **ID_HHNOTIFICATION**.
    *   To define a symbol, right-click the high-level folder in **ResourceView** and select **Resource Symbols**.
    *   In the **Resource Symbols** dialog box, click **New** and define the new symbol.
2.  In your Visual C++ project, initialize the **HH_WINTYPE** structure and call the **HTMLHelp** function to set this structure using the **HH_SET_WIN_TYPE** command. Use **ID_HHNOTIFICATION** for the _idNotify_ field in the structure.
3.  Override the **OnNotify** function in the derivative of the **CWnd** class that you want to receive the message (the **CWnd** class associated with **HWND** specified in the **hwndCaller** field of the **WW_WINTYPE** structure). The following example shows how an **OnNotify** function is used to call an **OnNavComplete(HHN_NOTIFY*, LRESULT)** handler whenever HTML Help navigates to a topic:

<pre> <font face="Courier">BOOL CMyView::OnNotify(WPARAM wParam, LPARAM lParam, LRESULT* pResult)
	{
		 NMHDR* pNMHDR = (NMHDR*)lParam;
	    switch (pNMHDR->idFrom) {
	        case ID_HHNOTIFICATION:  // whatever id you placed in idNotify of HH_WINTYPE
	                if (pNMHDR->code == HHN_NAVCOMPLETE) {
	                    OnNavComplete((HHN_NOTIFY*) lParam, pResult);
	                    return TRUE;
	                }
	                break;
	        }
	    }
	    return CView::OnNotify(wParam, lParam, pResult);
	}</font> </pre>

#### <a name="Doc_12"></a>Addendum to AutoClik Tutorial Topics

The AutoClik tutorial topics "Overview of AutoClik Steps 1, 2, and 3" and "Implementing Multiple Dispatch Interfaces" should mention that the .frm file included in AutoClik sample Step 3 enables accessing the automation object via Visual Basic.

#### <a name="Doc_13"></a>Tree View Controls Not Documented

Two Tree View Control styles were not documented at the time of shipping:

##### Non-even height

The height of the items can be set to an odd height with the TVM_SETITEMHEIGHT message. By default, the height of items must be an even value.

##### Right-to-left reading order

Displays text using right-to-left reading order on Hebrew or Arabic systems.

#### <a name="Doc_15"></a>References to MFC Version 4.22 in the Documentation

There are references to MFC version 4.22 in the "Porting and Upgrading" section of the _Visual C++ Programmer's Guide_ and in the section "Microsoft Foundation Class Library (MFC)" under _What's New in Visual C++ Version 6.0_. These references are incorrect and will be changed to 4.21\. There was no MFC version 4.22.

#### <a name="Doc_17"></a>wmemchr, wmemmove, wmemcpy, wmemset Not Available from C

The _Standard C++ Library Reference_ indicates that wmemchr, wmemmove, wmemcpy, wmemset, and so on, are available from C. Microsoft's implementation supports them only in C++, not in C.

#### <a name="Doc_18"></a>Undocumented CTabCtrl Styles

The **CTabCtrl** styles **TCS_BOTTOM**, **TCS_HOTTRACK**, and **TCS_VERTICAL** are not documented. These should be listed with the other valid styles in the **CTabCtrl::Create** topic. For descriptions of these styles, search online, with **Search titles only** selected, for the topic "Tab Control Styles" (under Platform SDK documentation) in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="Doc_19"></a>CControlBar::GetDockingFrame Documentation Does Not State Return Value When Control Bar Is Floating

The documentation for **CControlBar::GetDockingFrame** should state that if the control bar is not docked to a frame window (that is, if the control bar is floating), this function will return a pointer to its parent **CMiniFrameWnd**.

#### <a name="Doc_20"></a>Addendum to DECLARE_CLASSFACTORY_AUTO_THREAD Topic

The documentation for DECLARE_CLASSFACTORY_AUTO_THREAD should state the following:

When you wish to create objects in multiple apartments (in an out-of-proc server), add the macro **DECLARE_CLASSFACTORY_AUTO_THREAD** to your class and derive your EXE module from **CComAutoThreadModule**.

#### <a name="Doc_21"></a>Error in "CComModule::Init" Topic

The documentation for CComModule::Init omits the final parameter. This is the correct description:

**HRESULT Init(_ATL_OBJMAP_ENTRY* p, HINSTANCE h, const GUID* plibid = NULL)**

**<font color="NAVY">Return Value</font>**

A standard HRESULT value.

**<font color="NAVY">Parameters</font>**

_p_  
[in] A pointer to an array of object map entries.

_h_  
[in] The HINSTANCE passed to DLLMain or WinMain.

_plibid_  
[in] A pointer to the LIBID of the typelibrary associated with the project.

**<font color="NAVY">Remarks</font>**

Initializes all data members.

**See Also**   CComModule::Term

#### <a name="Doc_23"></a>Errors in "Implementing a Simple Consumer" Topic

The topic "Implementing a Simple Consumer" under "OLE DB Templates" in _Microsoft Foundation Classes and Templates_ has the following errors:

*   The topic "Implementing a Simple Consumer" should state:

Because you are manually creating this code, you need to include these in stdafx.h:

<pre> <font size="2">#include <atlbase.h>
extern CComModule _Module;
#include <atlcom.h>
#include <atlhost.h>
#include <atldb.h>
#include <atldbcli.h></font> </pre>

*   In "Add a handler for the Run button," the code should be changed as follows:

<pre> <font size="2" face="Verdana">From:</font> 
 <font size="2" face="Courier">if (source.Open("MyProvider.MyProvider.1", NULL) != S_OK)</font> 
 <font size="2" face="Verdana">To:</font> 
 <font size="2" face="Courier">if (source.Open("MyProvider.MyProvider.1") != S_OK)</font> 
 <font size="2" face="Verdana">After these changes are made, TestProv can be used to test MyProv.</font> 
</pre>

Also, there should be a space between the '>>' angle brackets in the line:

<pre> <font size="2" face="Verdana">From:</font> 
 <font size="2" face="Courier">CCommand<CAccessor<CProvider>> table;</font> 
 <font size="2" face="Verdana">To:</font> 
 <font size="2" face="Courier">CCommand<CAccessor<CProvider> > table;</font> 
</pre>

#### <a name="Doc_24"></a>Addendum to CProgressCtrl Topic

The documentation for **CProgressCtrl** suggests that the progress bar can display text. In fact, the current version of the progress bar does not draw text.

#### <a name="Doc_25"></a>Error in "Implementing a Window with CWindowImpl" Topic

In the topic "Implementing a Window with CWindowImpl," in the code example under the section "Superclassing an Existing Windows Class," the call to **DECLARE_WND_SUPERCLASS** lists the parameters in the reverse order. The seventh line of code should read:

<pre> <font size="2" face="Courier">DECLARE_WND_SUPERCLASS("MyEdit",  "Edit")</font> </pre>

#### <a name="Doc_26"></a>Errors in CDC::Escape Topic

The syntax for **CDC::Escape** should appear as follows:

<pre> <font size="2" face="Courier">virtual int Escape( int nEscape, int nCount, LPCSTR lpszInData, LPVOID lpOutData );
int Escape( int nEscape, int nInputSize, LPCSTR lpszInputData, int nOutputSize, LPSTR lpszOutputData );</font> </pre>

This member function is practically obsolete for Win32 programming. Of the original printer escapes, only QUERYESCSUPPORT is supported for Win32 applications. All other printer escapes are obsolete and are supported only for compatibility with 16-bit applications.

For Win32 programming, **CDC** now provides six member functions that supersede several printer escapes:

*   **CDC::AbortDoc**
*   **CDC::EndDoc**
*   **CDC::EndPage**
*   **CDC::SetAbortProc**
*   **CDC::StartDoc**
*   **CDC::StartPage**

In addition, **CDC::GetDeviceCaps** supports Win32 indexes that supersede other printer escapes. For more information, search online, with **Search titles only** selected, for the topic "GetDeviceCaps" in the _Platform SDK_ in the MSDN Library Visual Studio 6.0 documentation.

This member function allows applications to access facilities of a particular device that are not directly available through GDI.

Use the first version if your application uses predefined escape values. Use the second version if your application defines private escape values. For more information about the second version, search online, with **Search titles only** selected, for the topic "ExtEscape" in the _Platform SDK_ in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="Doc_27"></a>ATLCOLUMNINFO Structure Not Documented

**ATLCOLUMNINFO** is a structure defined by OLE DB Provider Templates in ATLDB.h. It contains the same fields as the **DBCOLUMNSINFO** structure defined by the OLE DB SDK with one additional field, cbOffset, that is used by ATL.

<pre> <font size="2" face="Courier">struct ATLCOLUMNINFO
{
	LPOLESTR pwszName;  	
	ITypeInfo *pTypeInfo;	
	ULONG iOrdinal;		
	DBCOLUMNFLAGS dwFlags;	
	ULONG ulColumnSize;	
	DBTYPE wType;		
	BYTE bPrecision;		
	BYTE bScale;		
	DBID columnid;		
	UINT cbOffset;		
};</font> </pre>

<pre> <font size="2" face="Verdana">**UINT** _cbOffset_ :	Byte offset for the column into the data buffer.
		Primarily used by **IRowsetImpl::GetData()**.</font> </pre>

For documentation of **DBCOLUMNSINFO** refer to the **IColumnsInfo::GetColumnInfo** topic in the _OLE DB Reference_.

#### <a name="Doc_28"></a>ATLTRACE and AtlTrace Documentation Incorrectly Refer to Dump Device

The **ATLTRACE** and **AtlTrace** documentation states that the _exp_ argument is "the formatted string and variables to send to the dump device." In fact, **ATLTRACE** and **AtlTrace** wrap the Win32 API **OutputDebugString**, the output of which is captured by the Visual C++ output window or any application that traps these messages.

#### <a name="Doc_29"></a>Errors in "How Do I Reference a Property in My Provider?" Topic

In the topic "How Do I Reference a Property in My Provider?" (in the _Microsoft Foundation Class Library and Templates, OLE DB Templates_) the following lines should be omitted:

<pre> <font size="2" face="Verdana">Use the data member _m_spUnkSite_ to get the pointer to the object that created your object.</font>  <font face="Courier">CAgentRowset<cmyprovidercommand>* pRowset = (CAgentRowset<cmyprovidercommand>*) pThis;

	CComQIPtr <irowsetinfo, &iid_irowsetinfo="">spRowsetProps = pRowset;</irowsetinfo,> </cmyprovidercommand></cmyprovidercommand></font></pre>

The following line should be inserted directly before the call to set.AddPropertyID in "Here's the final code."

<pre> <font face="Courier">DBPROPIDSET set;</font> </pre>

#### <a name="Doc_31"></a>Undocumented Function AfxDebugBreak

**<font size="4" color="GRAY">AfxDebugBreak</font>**

**void AfxDebugBreak( );**

**<font color="NAVY">Remarks</font>**

Call this function to cause a break (at the location of the call to **AfxDebugBreak**) in the execution of the debug version of your MFC application. **AfxDebugBreak** has no effect in release versions of an MFC application and should be removed. This function should only be used in MFC applications. Use the Win32 API version, **DebugBreak**, to cause a break in non-MFC applications.

#### <a name="Doc_32"></a>Undocumented ATL Consumer Method CDataSource::OpenWithServiceComponents

**OpenWithServiceComponents** was added to support the new OLE DB Service Components for cursoring, auto transaction enlistment and session pooling. It is used by both the MFC AppWizard and ATL Consumer Wizard-generated code.

**<font size="4" color="GRAY">CDataSource::OpenWithServiceComponents</font>**

**HRESULT OpenWithServiceComponents(const CLSID& clsid, DBPROPSET* pPropSet = NULL, ULONG nPropertySets=1)**

**HRESULT OpenWithServiceComponents(LPCTSTR szProgID, DBPROPSET* pPropSet = NULL, ULONG nPropertySets=1)**

**<font color="NAVY">Return Value</font>**  
A standard HRESULT.

**<font color="NAVY">Parameters</font>**  

_clsid_  
[in] The CLSID of the data provider.

_pPropSet_  
[in] A pointer to a DBPROPSET structure containing properties and values to be used to initialize the provider. The properties must belong to the Initialization property group. See CDBPropSet for further information.

_szProgID_  
[in] A program identifier.

_nPropertySets_  
[in] The number of DBPROPSET structures in pPropSet. If this is zero, the provider ignores pPropSet and the method does not do anything.

**<font color="NAVY">Remarks</font>**  
Opens a connection to a data source using a CLSID or program ID and utilizes the OLE DB Service Components which can provide cursoring, auto transaction enlistment and session pooling.

Service component documentation can be found in OLEDB SDK 2.0 readme.For an example of how to use this function generate an MFC Appwizard application and select OLE DB database support. Then examine the generated Open function in the C<YourProjectName>Set class.

#### <a name="Doc_33"></a>Errors in AddProject Method Topic

In the "Developer Studio Objects" reference in the _Visual C++ Users Guide_ the syntax of the AddProject method is incorrectly documented. Instead of:

<pre> <font size="2" face="Verdana">object.AddProject "project name" "project directory" "project type" addfolders

it should read:

	object.AddProject project name, project directory, project type, addfolders</font> </pre>

The commas are mandatory, or you get a syntax error. The quote marks should be removed for consistency with other samples. They are correctly documented as strings. The following is a code example using AddProject:

<pre><font size="2" face="Courier">Sub AddMyFile
Application.AddProject "MyProj", "c:\myproj", "Console Application", True
End Sub</font> </pre>

#### <a name="Doc_34"></a>Addendum to Documentation for Microsoft UpDown Control

The Microsoft UpDown Control is a Registered ActiveX Controls in the Gallery. The Gallery documentation should state that the UpDown control is limited to use on VB forms. The control relies on the Visual Basic implementation of extended properties like "Tab Index" and "Name." Because the VC++ resource editor does not support these properties, this control will not work with an MFC dialog app. This applies to the following Registered ActiveX Controls:

*   Microsoft UpDown Control, version 5.0 (ships with VC5)
*   Microsoft UpDown Control, version 6.0 (ships with VC6)

#### <a name="Doc_30"></a>Errors in "IDispatchImpl" and "IProvideClassInfo2Impl" Topics

The documentation of the classes **IDispatchImpl** and **IProvideClassInfo2Impl** should mention that you don't need to pass the LIBID as a template parameter. Following are the correct class descriptions.

**<font size="4" color="GRAY">IProvideClassInfo2Impl</font>**

**template < const CLSID* pcoclsid, const IID* psrcid, const GUID* plibid = &CComModule::m_libid, WORD wMajor = 1, WORD wMinor = 0, class tihclass = CComTypeInfoHolder > class ATL_NO_VTABLE IProvideClassInfo2Impl : public IProvideClassInfo2**

**<font color="NAVY">Parameters</font>**

_pcoclsid_  
A pointer to the coclass' identifier.

_psrcid_  
A pointer to the coclass' identifier.

_plibid_  
A pointer to the LIBID of the type library that contains information about the interface. By default, the server-level type library is passed.

_wMajor_  
The major version of the type library. The default value is 1.

_wMinor_  
The minor version of the type library. The default value is 0.

_tihclass_  
The class used to manage the coclass' type information. The default value is CComTypeInfoHolder.

**<font size="4" color="GRAY">IDispatchImpl</font>**

**template < class T, const IID* piid, const GUID* plibid = &CComModule::m_libid, WORD wMajor = 1, WORD wMinor = 0, class tihclass = CComTypeInfoHolder > class IDispatchImpl : public T**

**<font color="NAVY">Parameters</font>**

_T_  
A dual interface.

_piid_  
A pointer to the IID of T.

_plibid_  
A pointer to the LIBID of the type library that contains information about the interface. By default, the server-level type library is passed.

_wMajor_  
The major version of the type library. The default value is 1.

_wMinor_  
The minor version of the type library. The default value is 0.

_tihclass_  
The class used to manage the type information for T. The default value is CComTypeInfoHolder.

#### <a name="Doc_10"></a>CFileDialog Undocumented Functions

The following member functions are not included in the _Microsoft Fountation Class Library_ in the online Visual C++ documentation:

**<font size="4" color="GRAY">CFileDialog::GetFolderPath</font>**

**CString GetFolderPath( ) const;**

**<font color="NAVY">Return Value</font>**  
A CString object containing the currently open folder or directory.

**<font color="NAVY">Remarks</font>**  
Call this member function to retrieve the path of the currently open folder or directory for an Explorer-style **Open** or **Save As** common dialog box. The dialog box must have been created with the OFN_EXPLORER style; otherwise, the function will fail with an assertion.

**<font color="NAVY">See Also</font>**  
**CDM_GETFOLDERPATH**

**<font size="4" color="GRAY">CFileDialog::HideControl</font>**

**void HideControl( int nID );**

**<font color="NAVY">Parameters</font>**

_nID_  
The ID of the control to hide.

**<font color="NAVY">Remarks</font>**  
Call this member function to hide the specified control in an Explorer-style **Open** or **Save As** common dialog box. The dialog box must have been created with the OFN_EXPLORER style; otherwise, the function will fail with an assertion.

**<font color="NAVY">See Also</font>**  
**CDM_HIDECONTROL**

**<font size="4" color="GRAY">CFileDialog::SetControlText</font>**

**void SetControlText( int nID, LPCSTR lpsz );**

**<font color="NAVY">Parameters</font>**

_nID_  
The ID of the control for which to set the text.

_lpsz_  
A pointer to the string containing the text to set for the control.

**<font color="NAVY">Remarks</font>**  
Call this member function to set the text for the specified control in an Explorer-style **Open** or **Save As** common dialog box. The dialog box must have been created with the OFN_EXPLORER style; otherwise, the function will fail with an assertion.

**<font color="NAVY">See Also</font>**  
**CDM_SETCONTROLTEXT**

**<font size="4" color="GRAY">CFileDialog::SetDefExt</font>**

**void SetDefExt( LPCSTR lpsz );**

**<font color="NAVY">Parameters</font>**

_lpsz_  
A pointer to a string containing the default extension to use for the dialog box object. This string must not contain a period (.).

**<font color="NAVY">Remarks</font>**  
The CDM_SETDEFEXT message sets the default file name extension for an Explorer-style **Open** or **Save As** common dialog box. The dialog box must have been created with the OFN_EXPLORER style; otherwise, the function will fail with an assertion.

**<font color="NAVY">See Also</font>**  
**CDM_SETDEFEXT**

**<font size="4" color="GRAY">CFileDialog::SetTemplate</font>**

**void SetTemplate( UINT nWin3ID, UINT nWin4ID );  
void SetTemplate( LPCTSTR lpWin3ID, LPCTSTR lpWin4ID );**

**<font color="NAVY">Parameters</font>**

_nWin3ID_  
Contains the ID number of the non-Explorer common file dialog template resource. This template is only used on Windows NT 3.51 or when the OFN_EXPLORER style is not present.

_nWin4ID_  
Contains the ID number of the Explorer common file dialog template resource. This template is only used on Windows NT 4.0 or greater, Windows 95 or greater, or when the OFN_EXPLORER style is present.

_lpWin3ID_  
Contains the name of the non-Explorer common file dialog template resource. This template is only used on Windows NT 3.51 or when the OFN_EXPLORER style is not present.

_lpWin4ID_  
Contains the name of the Explorer common file dialog template resource. This template is only used on Windows NT 4.0 or greater, Windows 95 or greater, or when the OFN_EXPLORER style is present.

**<font color="NAVY">Remarks</font>**  
Call this function to set the dialog box template for the CFileDialog object. Only one of the specified templates is used, depending on the presence of the OFN_EXPLORER style and depending on the platform that the application is running on. By specifying both a non-Explorer and Explorer-style template, it is easy to support Windows NT 3.51, Windows NT 4.0 and greater, and Windows 95 and greater.

### <a name="ActiveX_Control_Issues_0"></a>ActiveX Control Issues

#### <a name="ActiveX_Control_Issues_1"></a>New ActiveX Control Test Container Cannot Open Saved Sessions Files Created by Previous Version

The ActiveX control test container cannot open saved sessions (*.tcs) files created in previous test container versions. If you try to open a session from the previous November Pre-Release version of test container, the test container will crash. However, from now on your ambient property settings will be saved with the session.

#### <a name="ActiveX_Control_Issues_2"></a>Problems Accessing ActiveX Control Test Container Help

Context-sensitive (F1) help will not be available in the ActiveX Control Test Container when you first access it. You will get an error stating:

<pre><font size="2" face="Courier">The topic does not exist. Contact your application vendor for an updated help file. (129)</font></pre>

To work around this problem:

1.  Delete TstCon32.cnt from the Common\Tools directory of your installation. Then find any hidden files on your hard drive named TstCon32.gid and delete them as well.
2.  Change the line in Samples\MFC\OLE\TstCon\Hlp\TstCon.hpj that reads:

<pre> <font size="2" face="Verdana">HIDR_MAINFRAME = main_index

to

	HIDR_MAINFRAME=_ASUG_Contents</font></pre>

4.  Rebuild and replace the help file in the Common\Tools directory.

#### <a name="ActiveX_Control_Issues_4"></a>Some ActiveX Controls Created with Visual Basic Generate Error in Test Container on Resize

You can create ActiveX Controls (OCX's) with Microsoft Visual Basic<sup>®</sup> 5.0\. Some controls that are created with Visual Basic set the OLEMISC_NOUIACTIVATE bit. If you insert the control into the ActiveX control test container and then resize it, the test container attempts a DoVerb (OLEIVERB_UIACTIVATE) call that results in the following error:

"Failed to connect. Link may be broken."

This problem is being investigated. This does not impede hosting the control in Visual C++.

#### <a name="ActiveX_Control_Issues_5"></a>Oracle Joins and MSRDC20.ocx (Remote Data Control V2)

If you use the Microsoft ODBC Driver for Oracle with the Microsoft Remote Data Control (MRDC20.ocx) and your SQL statement contains a join (or includes a reference to a view that contains a join), you may encounter the following driver error:

"SC100: [Microsoft][ODBC Driver for Oracle]Driver not capable"

##### Workaround

Change the **CursorDriver**, **LockType**, and **ResultsetType** properties as follows.

CursorDriver = 'ODBC Cursor'

LockType = ' Optimistic Concurrency'

ResultsetType = 'Create a Static Cursor'

#### <a name="ActiveX_Control_Issues_6"></a>Current, Localized ActiveX Redistributable Components

The ActiveX redistributable components that ship with Visual C++ 6.0 were current when the product was released to manufacturing. Check [http://www.microsoft.com/intdev/sdk/](http://www.microsoft.com/intdev/sdk/) for the most current components.

**Note**   If your Internet application will be used in an Internet Explorer localized environment, your application should use the localized ActiveX components that are available from this site, otherwise the components contained on this CD-ROM may overwrite Internet Explorer localized components.

### <a name="Language_Issues_0"></a>Language Issues

#### <a name="Language_Issues_3"></a>Size Mismatch for Type bool in Visual C++ 4.2 Programs Built with Visual C++ 6.0

In Visual C++4.2, the Standard C++ header files contained a **typedef** that equated **bool** with **int**. In Visual C++ 6.0, **bool** is implemented as a built-in type with a size of 1 byte. This means that for Visual C++ 4.2, a call of sizeof(bool) yields 4, while in Visual C++ 6.0, the same call yields 1\. This can cause memory corruption problems if you have defined structure members of type **bool** in Visual C++ 4.2 and are mixing object files (OBJ) and/or DLLs built with the 4.2 and 6.0 compilers.

#### <a name="Language_Issues_4"></a>Support for Member Templates

C++ member templates are supported as long as they are fully defined within the enclosing class. For example, the following is supported:

<pre> <font face="courier">template<typename T&>
   class X {
   public:
      template<typename U>
      void mf(const U &u) {
         // ...
      }
   };</font> </pre>

while the following is not:

<pre> <font face="courier">template<typename T>
   class X {
   public:
      template<typename U>
      void mf(const U &u);
   };

   template<typename T>
   template<typename U>
   void X<T>::mf(const U &)
   {
      // ...
   }</font> </pre>

### 

<a name="MFC_0"></a>Libraries Issues

#### <a name="MFC_1"></a>Using MFC with New SDK Releases

Upgrading SDKs and system components wrapped by MFC can cause compatibility problems. MFC strives to be backward compatible. However, if new components are installed on your system, they may no longer be compatible with MFC or MFC may simply be unaware of them.

#### <a name="MFC_3"></a>Incomplete Documentation for CWnd::RepositionBars

The documentation for **CWnd::RepositionBars** is missing the parameter _bStretch_. The prototype should read:

**void RepositionBars( UINT** _nIDFirst_**, UINT** _nIDLast_**, UINT** _nIDLeftOver_**, UINT** _nFlag_ **= reposDefault, LPRECT** _lpRectParam_ **= NULL, LPCRECT** _lpRectClient_ **= NULL, BOOL** _bStretch_ **= TRUE );**

_bStretch_ indicates whether the bar should be stretched to the size of the frame.

#### <a name="MFC_5"></a>Incorrect Example Code in the CArchive::MapObject Member Function

In the SubItem.cpp section of the **CArchive::MapObject** member function code, nonexistent overloaded **CDocument** operators (<< and >>) are used in two places. This code section should be replaced with the following code:

<pre> <font face="courier">//SubItem.cpp

void CSubItem::Serialize(CArchive& ar)

{
if (ar.IsStoring( ) )
{

// will serialize a reference 
// to the "mapped" document pointer

ar << (CObject *)m_pDoc;
ar << m_l;
}

else

{

// Will load a reference to
// the "mapped" document pointer

ar >> (CObject *&) m_pDoc;
ar >> m_l;
}
}</font> </pre>

#### <a name="MFC_5.1"></a>Some ATL Object Stock Properties Must Be Initialized Before Use in Visual Basic 5.0 Containers

Visual Basic 5.0 expects all stock properties that are **IUnknown**-based (such as MousePointer, Picture, and Font) to contain a valid **IUnknown** pointer. Otherwise, Visual Basic will not allow the user to change the property. For example, if you have a stock Font property that you never fill in with a valid Font, Visual Basic will display the Font as being **NULL**, and will not allow the user to select a new Font through the Visual Basic property window.

To avoid this problem, make sure your **IUnknown**-based stock properties have a valid value other than **NULL** before inserting your object into a Visual Basic container. There are many ways to do this, for example, get the ambient Font off the container and use that as your stock Font property.

#### <a name="MFC_5.3"></a>ATL Font and Picture Properties May Require Changes to the IDL File

To make a Font or Picture property work in some containers, you must declare the interface definition within the library section of the .idl file. Cut the interface declarations from the .idl file and paste them into the library section of the same file. In addition, you must comment out the import line for ocidl.idl.

For more information on this problem see Knowledge Base article Q166472, "FILE: Using Fonts in ATL Controls with NiceText.exe" in the Knowledge Base section of the MSDN Library Visual Studio 6.0 documentation.

#### <a name="MFC_6"></a>Documentation Missing for MFC Message Map Macro ON_WM_SETTINGCHANGE

The MFC message map entry ON_WM_SETTINGCHANGE corresponds to the following MFC message handler:

<font size="3" color="Gray">**CWnd::OnSettingChange**</font>

**afx_msg void OnSettingChange( UINT uFlags, LPCTSTR lpszSection );**

##### Parameters

<table width="637" cellspacing="0" cellpadding="7" border="0">

<tbody>

<tr>

<td width="14%" valign="TOP">

<font size="2">_uFlags_</font>

</td>

<td width="86%" valign="TOP">

<font size="2">When the system sends the message as a result of a **SystemParametersInfo** call, this parameter is a flag that indicates the system parameter that was changed. For a list of values, search online (with **Search titles only** selected) for the topic "SystemParametersInfo" in the _Platform SDK_ in the MSDN Library Visual Studio 6.0 documentation. When an application sends the message, this parameter must be 0.</font>

</td>

</tr>

<tr>

<td width="14%" valign="TOP">

<font size="2">_lpszSection_</font>

</td>

<td width="86%" valign="TOP">

<font size="2">Points to a string that specifies the name of the section that has changed. (The string does not include the square brackets that enclose the section name.)</font>

</td>

</tr>

</tbody>

</table>

##### Remarks

The framework calls **OnSettingChange** for all top-level windows when the Win32 **SystemParametersInfo** function changes a system-wide setting. An application should send the message to all top-level windows when it makes changes to system parameters, and Windows will send the message if the user changes settings via the Control Panel.

The **ON_WM_SETTINGCHANGE** message is similar to the **ON_WM_WININICHANGE** message, with the following difference:

*   Use **ON_WM_SETTINGCHANGE** when running Windows NT 4.0 or newer, or under Windows 95\.
*   Use **ON_WININICHANGE** when running Windows NT 3.51 or older. This message is now obsolete.

You should have only one of these macros in your message map. To write a program that works for both Windows 95 and Windows NT 4.0, write a handler for **ON_WM_SETTINGCHANGE**. Under Windows NT 3.51, your handler will be called by **OnSettingChange** and _uFlags_ and will always be zero.

**See Also   SystemParametersInfo** and **WM_SETTINGCHANGE** in the _Platform SDK_, and **ON_WININICHANGE** and **CWnd::OnWinIniChange** in the _Microsoft Foundation Class Library Reference_.

#### <a name="MFC_7"></a>TN024 Doesn't Identify All Custom MFC Resource Types

MFC Technote TN024, titled "MFC-Defined Messages and Resources", states:

"There is currently only one MFC private resource format defined, **RT_DLGINIT**."

This statement should read:

"Currently, MFC defines two private resource formats: **RT_DLGINIT** and **RT_TOOLBAR**."

The default toolbar supplied by AppWizard is based on an **RT_TOOLBAR** custom resource, which was introduced in MFC 4.0\.

You can edit this resource with the Toolbar editor.

#### <a name="MFC_8"></a>MFC DAO Classes Will Work with Either DAO 3.0 or DAO 3.5

However the MFC DAO classes have not been designed to take advantage of any new DAO 3.5 features, including ODBCDirect.

#### <a name="MFC_9"></a>Using DAO with a Secure Database

If you are writing a program that uses Data Access Objects (DAO) to access a secure database, you will receive an error if you use **CDaoRecordset** because MFC does not prompt the user for a their name and password. To find out how to call DAO directly to implement DAO security features, such as changing user passwords, search online, with **Search titles only** selected, for the topic "TN054: Calling DAO Directly While Using MFC DAO Classes" in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="MFC_10"></a>The Hewlett Packard Standard Template Library

Visual C++ 6.0 ships a complete, fully supported C++ Standard Run-time Library, that includes the Microsoft implementation of the Standard Template Library.

Setup installs the new C++ Standard Run-time Library with the other run-time libraries.

**Note** The Hewlett Packard Standard Template Library that shipped with Visual C++ 4.0 does not ship with Visual C++ 6.0\. Microsoft does not provide technical support for the Hewlett Packardversion of the Standard Template Library.

#### <a name="MFC_13"></a>MFC Loads Wrong Resource in Extension .dll

The wrong resource is loaded when **CBitmap::LoadBitmap**, **CMenu::LoadMenu**, **CString::LoadString** or any other MFC resource-loading function is called in an MFC extension .dll (AFXDLL). In some cases, a resource in the application is loaded instead of the appropriate resource in the extension .dll.

For more information on this problem see Knowledge Base article Q150121, "PRB: MFC Loads Wrong Resource in Extension DLL" in the Knowledge Base section of the MSDN Library Visual Studio 6.0 documentation.

#### <a name="MFC_14"></a>Call _findclose After Using _findfirst or _findnext

You must call _**findclose** after you are finished using either the _**findfirst** or **_findnext** function. This will free up resources used by these functions in your application.

#### <a name="MFC_20"></a>Format Specification Not Supported in COleDateTime and COleDateTimeSpan Classes

The description of the member function Format in both the **COleDateTime** and the **COleDateTimeSpan** erroneously states that you can use the %D format specification to display the number of days. Neither **COleDateTime::Format** nor **COleDateTimeSpan::Format** support that format specification.

#### <a name="MFC_21"></a>IsBadHugeReadPtr, IsBadHugeWritePtr, IsBadStringPtr, IsBadWritePtr, and Access Violations

A handled exception will occur inside of these functions if the specified memory region is not accessible to the process when these functions attempt to access it. If the code is being executed under a debugger, and the debugger is configured to get first chance at handling exceptions, the debugger will trap the access violation and stop program execution. At this point, you can simply continue execution in the debugger and these functions will return the appropriate value. This behavior can help you find potential access violations in your code.

#### <a name="MFC_23"></a>ServerSupportFunction No Longer Supports SF_REQ_GET_CONNID

Internet Information Server (IIS) versions 4.0 and later no longer support the function **SF_REQ_GET_CONNID**. You can no longer specify it in the MFC function **CHttpFilterContext::ServerSupportFunction**.

#### <a name="MFC_24"></a>Hot Track Property for Spin Control Not Implemented

The Hot Track property for the Spin Control is not implemented in Internet Explorer version 4.70\. The property is currently undocumented.

#### <a name="MFC_25"></a>COleDateTime::GetStatus Returns Valid for Default Constructor

As stated in the topic **COleDateTime::COleDateTime**, the default constructor initializes to zero and valid. If you call **COleDateTime::GetStatus** on a **COleDateTime** object constructed with the default, it will return valid. **GetStatus** will return null only if you initialized the constructor to null.

#### <a name="MFC_26"></a>Opening a DLL as "Resources" Might Require Installation of .nls Files

If you open a DLL to use its resources, you might get a message box that says a certain code page is required to support a foreign language. For example, if you open COMCTL32.DLL as "resources," you get a message box that says "Code page 950 is required to support a Chinese (Taiwan) language resource in this file."

In such a case, you will have to install national language support (.nls) files. See [Multiple Language Resource Files](#MFC_27) for details.

#### <a name="MFC_27"></a>Multiple Language Resource Files

Visual C++ allows your resource file to contain resources in multiple languages. This is useful if you work on a global application which supports multiple languages in its user interface. One requirement for using such resources on your machine is that you have the appropriate national language support (.nls) files. Since specific localized versions of Windows 95/98 and Windows NT do not contain the .nls files you may need, there are several .nls files on the OS CD-ROM which enable you to work with multiple language resource files.

As an example, consider an application which can be built so that its user interface elements (resources) are in Japanese or English. Typically, one person working on a US Windows 95/98 or Windows NT machine works on the English resources, while another person on a Japanese Windows 95/98 or Windows NT machine works on the Japanese resources. Since both the Japanese and English resources are in the same file, it is important that the US machine load up and edit the English resources without corrupting the Japanese resources. In order to do this, the US machine must have the Japanese .nls files installed. It is important to distinguish between being able to load up a resource file which contains resources that are not in the primary language of the machine, and actively working on these resources. Actively working on the Japanese resources does require a Japanese machine, since input of Japanese characters requires an input method editor (IME), and you must have the correct fonts in order to display these characters appropriately, and for correct caret placement. However, just by having the Japanese .nls file on the US machine you can load up your .rc file, work on the US resources, and save it back while maintaining the integrity of the Japanese resources section.

The following .nls files are available on the OS CD-ROM:

<pre><font size="2" face="Verdana">**Code Page	Language (script)		Filename (Windows 95/98)	Filename (Windows NT)**
932		Japanese				cp_932.nls			c_932.nls
936		Simplified Chinese			cp_936.nls			c_936.nls
949		Unified Hangul			cp_949.nls			c_949.nls
950		Traditional Chinese			cp_950.nls			c_950.nls
1250		Central / Eastern European		cp_1250.nls			c_1250.nls
1251		Cyrillic				cp_1251.nls			c_1251.nls
1252		Latin I				cp_1252.nls			c_1252.nls
1253		Greek				cp_1253.nls			c_1253.nls
1254		Turkish				cp_1254.nls			c_1254.nls
1255		Hebrew				cp_1255.nls			c_1255.nls
1256		Arabic				cp_1256.nls			c_1256.nls
1257		Baltic				cp_1257.nls			c_1257.nls</font> </pre>

##### Installing the National Language Support Files on Windows 95/98

_Run the registry editor (RegEdit):_

The key My Computer \ HKEY_LOCAL_MACHINE \ System \ CurrentControlSet \ control \ Nls \ Codepage lists all the code pages that are installed, and can be installed on your system. Note that in this key, the value name specifies the code page, and the value data specifies the file which contains the code page information. Installed code pages have an entry for value data, whereas code pages that are not installed do not specify an entry in the value data field.

To install additional code pages, first copy the appropriate .nls file(s) from your OS CD-ROM into the Windows system directory. This is the SYSTEM subdirectory under your Windows directory.

Second, in the appropriate registry key (see above), select the codepage entry for the file you just copied. Select Modify from the Edit menu (or double click the codepage entry) to bring up the Edit String dialog box. Enter the name of the file you just copied in the value data field. Click the OK button.

Close the registry editor. You have completed the installation of the additional code pages.

##### Installing the National Language Support Files on Windows NT

_Run the registry editor (regedt32):_

The HKEY_LOCAL_MACHINE \ System \ CurrentControlSet \ Control \ Nls \ Codepage key lists all the code pages that are installed, and can be installed on your system. Note that in this key, the value name specifies the code page, and the value data specifies the file which contains the code page information. The value data is of type REG_SZ. Installed code pages have an entry for value data, whereas code pages that are not installed do not specify an entry in the value data field.

To install additional code pages, first copy the appropriate .nls file(s) from your OS CD-ROM into the Windows system directory. This is the SYSTEM32 subdirectory under your Windows directory.

Second, in the appropriate registry key (see above), select the codepage entry for the file you just copied. Select String from the Edit menu (or double click the codepage entry) to bring up the String Editor. Enter the name of the file you just copied in the string edit field. Click the OK button.

Close the registry editor. You have completed the installation of the additional code pages.

#### <a name="MFC_28"></a>AfxDumpStack API Will Not Work until NT 5.0 Beta 2

The MFC function **AfxDumpStack** will work correctly only on Windows NT 5.0 Beta 2 or later. Once this OS version is released, you can get imagehlp.dll from your NT installation and use it on other OS installations to get the functionality of **AfxDumpStack** to work correctly.

#### <a name="MFC_29"></a>Changes to IObjectSafetyImpl

Because of changes to **IObjectSafetyImpl**, you will get several compiler errors when you build an ATL 2.1 project in ATL 3.0\. You'll need to make the changes listed under **IObjectSafetyImpl** in "Porting from ATL 2.1" in "Microsoft Foundation Class Library and Templates."

**Note**   In addition to these changes, the member variable m_dwSafety has been changed to m_dwCurrentSafety.

#### <a name="MFC_30"></a>Some Concrete MFC Classes Have No vtable When Built, Causing GPF on Deletion

The following classes are logically abstract and intended to be derived from rather than be directly instantiated. They are declared AFX_NOVTABLE in the static release version of MFC and will consequently will have no vtables. Use of these classes when directly instantiated is unpredictable. The solution is to use your own derived class.

*   CDocument
*   CCmdTarget
*   CException

For example, the following code will crash when built with the static release version of the library:

<pre><font size="2" face="Courier">try
{
   throw new CException;
}
catch(CException* pe)
{
   pe->Delete();
}

	// or

TRY
{
   throw new CException;
}
CATCH(CException, pe)
{
}
END_CATCH</font> </pre>

### <a name="Wizards_0"></a>Wizard and Other User-Interface Issues

#### <a name="Wizards_2"></a>Using the MTS Option in ATL COM AppWizard

Selecting the **Support MTS** option adds a custom build step that directs you to execute mtxrereg.exe before using the component in MTS (in addition to running regsvr32).

The ATL COM component will still be registered correctly and can be debugged on the machine. However, unless you run mtsrereg.exe after registering the component, you might observe aberrant behavior when you try to run the ATL COM component within MTS.

#### <a name="Wizards_2.15"></a>Save .idl File Before Invoking ATL Add Method or ATL Add Property

Before invoking **Add Property** or **Add Method** on an ATL class, you should first save the .idl file. This enables the parser to identify the correct location of all elements in the file.

#### <a name="Wizards_2.16"></a>Databinding Dialog Controls in an OLE DB Application

ClassWizard does not support **COleDBRecordView**, so you cannot use ClassWizard to do the databinding (message maps) in an OLE DB application.

To databind the controls in an OLE DB application, use dialog data exchange (DDX) data calls with **COleDBRecordView** just as you would with any other MFC class. You will need to add lines to the recordset file such as:

<pre> <font face="Courier">DDX_Text(pDX, IDC_EDIT1, m_pSet->m_nFoo); // if it's a LONG</font> 
 <font size="2" face="Verdana">-or-</font>
 <font face="Courier">DDX_Text(pDX, IDC_EDIT1, m_pSet->m_nFoo, 50); // If it's a char 50 array</font>
</pre>

The MFCRows sample demonstrates how to use **COleDBRecordView** to scroll through a table in a database. It also demonstrates how to use multiple accessors so that an update can be performed on an Access table that contains an AutoNumber field that is being retrieved. The sample is located in \Samples\VC98\MFC\database\MFCRows on the MSDN CD-ROM.

#### <a name="Wizards_2.18"></a>MFC AppWizard Generated Code Needs Editing for Tables and Providers with Spaces in Names

When you choose the MFC AppWizard OLEDB data option, and you choose a table name or provider with spaces embedded in the name, you must modify the generated code in the following fashion:

<pre><font size="2" face="Verdana">The name of the table or provider has to be surrounded in escaped quotes:

	before:   "select * from \"table name with space\"" 
	after:  "select * from \"table name with space\""

If the appwizard inserts double escapes, the doubles have to be removed:

	before:  "\\"table name\\""
	after:  "\"table name\""</font> </pre>

#### <a name="Wizards_6"></a>Two New Template Variables Available to Custom AppWizards

<table width="638" cellspacing="0" cellpadding="7" border="0">

<tbody>

<tr>

<td width="18%" valign="TOP">

<font size="2">root_oem</font>

</td>

<td width="82%" valign="TOP">

<font size="2">Same as 'root' except translated to the OEM character set. Affects only upper ASCII characters in the project name (such as an umlauted character).</font>

</td>

</tr>

<tr>

<td width="18%" valign="TOP">

<font size="2">HM_FILE_OEM</font>

</td>

<td width="82%" valign="TOP">

<font size="2">Same as 'HM_FILE' except translated to the OEM character set. Affects only upper ASCII characters in the project name (such as an umlauted character).</font>

</td>

</tr>

</tbody>

</table>

The Visual C++ tools work with the ANSI character set. Batch files, such as makehelp.bat, work with the OEM character set--a legacy from the days of DOS 1.0 that still exists. Most printable characters in these two sets are the same. However, there are some differences in some of the upper ASCII values used for European characters, such as those that use an umlaut.

#### <a name="Wizards_7"></a>Problems with ClassWizard-Generated Wrapper Classes for Visual Basic 5 ActiveX Servers

With Visual Basic 5.0 you can create ActiveX Automation servers with methods that can take Optional and Default parameters of any Visual Basic intrinsic type. If you use MFC and want to access an object of a Visual Basic ActiveX Automation server, you would typically use ClassWizard to read the type information of the Visual Basic object and generate a class that wraps the functionality of the Visual Basic Automation object. C++ does not have optional or default parameters; consequently, the wrapper class that ClassWizard generates will not mark parameters as Optional or Default.

For example, if you have a Visual Basic Server with the following function:

<pre> <font face="courier">Function function2(Optional parm1 As Integer = 5)

MsgBox parm1

End Function</font> </pre>

ClassWizard will generate the following C++ wrapper function:

<pre> <font face="courier">VARIANT _MyVBObj::function2(short* parm1)

{

 VARIANT result;

 static BYTE parms[] = VTS_PI2;

 InvokeHelper(0x60030001, DISPATCH_METHOD, VT_VARIANT,

  (void*)&result, parms, parm1);

 return result;

}</font> </pre>

If you call the ClassWizard-generated function from your MFC program, you will have to pass the argument even though Visual Basic marked it as Optional.

##### **Workaround**

Override the function that ClassWizard generates with versions of the function that take only the parameters you wish to pass. For example, in the preceding case, if you didn't want to pass the optional parameter, override the ClassWizard generated function as follows:

<pre> <font face="courier">VARIANT _MyVBObj::function2()

{

 VARIANT result;

 InvokeHelper(0x60030001, DISPATCH_METHOD, VT_VARIANT,

  (void*)&result, NULL);

 return result;

}</font> </pre>

The default parameter for the Visual Basic server's function2 would be used.

#### <a name="Wizards_8"></a>ATL Controls in Visual Basic 5.0 Containers

If you're using the **IQuickActivate** interface in Visual Basic 5.0, you must also support **IPropertyNotifySink**.

To use a control generated by the ATL Object Wizard in a Visual Basic 5.0 container, you must either add support for **IPropertyNotifySink** or remove dependence on the **IQuickActivate** interface. To remove **IQuickActivate** support, comment out the lines containing **IQuickActivateImpl** in the control's class inheritance list and in the COM interface map.

For example, if you generate a Full Control called MyCtl with the ATL Object Wizard, then go to MyCtl.h and comment out the line containing **IQuickActivateImpl** in the CMyCtl class inheritance list:

<pre> <font face="courier">class ATL_NO_VTABLE CMyCtl :
...
// public IQuickActivateImpl<CMyCtl></font> </pre>

Also, comment out the line containing **IQuickActivateImpl** in the COM interface map in MyCtl.h:

<pre> <font face="courier">BEGIN_COM_MAP(CMyCtl)
...
// COM_INTERFACE_ENTRY_IMPL(IQuickActivate)</font> </pre>

#### <a name="Wizards_10"></a>ClassView's Add Method and Add Property Dialog Boxes Sometimes Allow Illegal Return Types for Custom Interfaces

The return type dropdown for **Add Method** and **Add Property** should be active only for dispinterfaces and for custom interfaces with the **local** attribute. The return type is fixed at **HRESULT** for all other interface definitions--such as dual. Unfortunately, it is active for all non-dual interfaces. The MIDL compiler will fail with error 2269 when you build your project if you change the return type to something other than **HRESULT** or **SCODE** for a property or method in a custom interface that doesn't have the **local** attribute.

#### <a name="Wizards_11"></a>MFC Header stdafx.h May Not Have All Necessary #include's from a Visual Modeler Code Generation

Microsoft Visual Modeler allows you to create object models, then to create Visual C++ projects based on those models. The following issue exists in the current version of Visual Modeler.

When you generate code from Visual Modeler into a Visual C++ project, Visual Modeler assumes that stdafx.h includes all of the MFC classes. Whether this is true depends on what options you choose from the MFC AppWizard. If you reference an MFC class not included in your project's stdafx.h file, you will receive a compiler error. You must manually edit stdafx.h and add the related #include's.

#### <a name="Wizards_13"></a>IntelliSense Does Not Display Class Members for Inline Member Functions

If your cursor is in a function that is defined inside a class, IntelliSense options will not be available for members of that class. You can still display Globals in the Members List, but members of the current class will be omitted from the list, and Parameter Help and Type Info will not appear. This does not apply to inline functions that are defined outside of a class.

#### <a name="Wizards_14"></a>IntelliSense Might Present Outdated Information with Operating Systems That Ship After Visual C++ 6.0

Statement completion information is generated from the system headers available at the time of shipment and therefore might be inaccurate or incomplete with any operating system that ships after Visual C++ 6.0.

#### <a name="Wizards_15"></a>IntelliSense Limitations

A listing of IntelliSense limitations is published in Knowledge Base Article Q153284.

#### <a name="Wizards_16"></a>ClassView's Implement Connection Point: Problem with DIIDs in the Connection Point Map

The Implement Connection Point wizard might place the wrong entry in the Connection Point Map. The incorrect entry uses IID_ISomeInterface instead of DIID_ISomeInterface. You can easily resolve this by modifying the entry to use DIID_ISomeInterface. If you use the wizard to update the same connection point interface, the wizard might put in a duplicate entry that will use IID_ISomeInterface. Just delete this duplicate entry from the map.

#### <a name="Wizards_17"></a>Help for All Tab in ActiveX Controls Properties Sheet Not Available

Help from the **All** tab in the Properties sheet for ActiveX controls is not available. To view the help topic for properties that might appear on the **All** tab, click the **More Info** button in the **Components and Controls Gallery** dialog box. (This is in the **Project** menu, **Add to Project** command, **Components and Controls** item.)

#### <a name="Wizards_18"></a>Notes for MMC Snapin Object in ATL Object Wizard

*   Do not select IPersistStorage for the Persistence type in the MMC Snapin wizard. IPersistStorage option does not work properly.
*   Snapin wizard uses RGB(0,128,128) as the transparent color for bitmaps. MMC and many other applications use RGB(255,0,255).
*   To display property pages, your snap-in must set the MMC_VERB_PROPERTIES verb to the ENABLED button state using the IConsoleVerb::SetVerbState method. MMC displays a Properties item in the context menu only if the snap-in enables MMC_VERB_PROPERTIES. Likewise, the other standard menu items (Cut, Copy, Paste, Rename, and so on) are displayed in the context menu only when their verbs are enabled.
*   An incorrect comment is generated in C*Data::Notify that states that the MMCN_SHOW handler should enumerate both scope and result items. MMCN_SHOW is sent to enumerate result items only. MMCN_EXPAND is sent to enumerate scope items.

#### <a name="Wizards_19"></a>ATL Control's HWND Stock Property Causes Error Dialog in VB

If you choose to support the stock property for an HWND in an ATL control, the ATL object wizard incorrectly adds the following line to the property map in an ATL control class header:

<pre> <font size="2" face="Courier">PROP_ENTRY("HWND", DISPID_HWND, CLSID_NULL)</font></pre>

This is a read-only property and this entry should be removed from the property map in the class declaration.

#### <a name="Wizards_20"></a>Program Does Not Compile When You Insert a New ATL Object into an MFC Database Application Using OLE DB Datasource

A program will fail to compile if you add ATL support (inserting an ATL object) into an MFC EXE application that has database support with an OLE DB data source. There is no workaround for this in Visual C++ 6.0.

#### <a name="Wizards_21"></a>Warning on ATL Object Wizard's "Free Threaded Marshaler" Option

Using the ATL Object Wizard's **Free Threaded Marshaler**option without understanding basic threading model concepts can cause severe side effects (such as system crashes or access violations). For more information on these consequences, see the Knowledge Base article Q150777\. Search online, with **Search titles only** selected, for the topic "INFO: Descriptions and Workings of OLE Threading Models" in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="Wizards_22"></a>Project Names with Upper-ASCII or DBCS Characters Cause Build Errors in Custom AppWizard-Generated Projects

When creating a Custom AppWizard, do not use upper-ASCII or DBCS characters (such as umlauted characters) in the project name. Such characters will cause build errors.

#### <a name="Wizards_23"></a>Assertion in AppWizard-Generated MDI Active Document Container

AppWizard-generated MFC MDI Active Document containers will assert when running under the debugger if an MDI document that contains an Active document is opened while another MDI document that contains an Active document is already open. This assertion fires because the first MDI active document is not completely in-place deactivated when the second MDI Active document container is opened. To avoid this problem, remove the AppWizard-generated in-place activation code from the view class' OnInitialUpdate. Also, create a WM_MDIACTIVATE Windows message handler in the MDI child frame class and in that handler, activate the contained MDI object. The following steps show how to fix the problem:

1.  Open the CView-derived class' .cpp file. From the OnInitialUpdate function, delete the following code:

<pre> <font face="Courier">//Active documents should always be activated
	COleDocument* pDoc = (COleDocument*) GetDocument();
	if (pDoc != NULL)
	{
		// activate the first one
		POSITION posItem = pDoc->GetStartPosition();
		if (posItem != NULL)
		{
			CDocItem* pItem = pDoc->GetNextItem(posItem);

			// only if it's an Active document
			COleDocObjectItem *pDocObjectItem =
				DYNAMIC_DOWNCAST(COleDocObjectItem, pItem);

			if (pDocObjectItem != NULL)
			{
				pDocObjectItem->DoVerb(OLEIVERB_SHOW, this);
			}
		}
	}</font></pre>

3.  In the CMDIChildWnd-derived class, use ClassWizard to add a Windows message handler for WM_MDIACTIVATE.
4.  In the OnMDIActivate function added in Step 2 above, add the following code to activate the first Active document contained in the Document/Frame/Views document.

<pre> <font face="Courier">CView *pView = GetActiveView();
	ASSERT_VALID(pView);
	//Active documents should always be activated
	COleDocument* pDoc = (COleDocument*) pView->GetDocument();
	if (pDoc != NULL)
	{
		// activate the first one
		POSITION posItem = pDoc->GetStartPosition();
		if (posItem != NULL)
		{
			CDocItem* pItem = pDoc->GetNextItem(posItem);

			// only if it's an Active document
			COleDocObjectItem *pDocObjectItem =
				DYNAMIC_DOWNCAST(COleDocObjectItem, pItem);

			if (pDocObjectItem != NULL)
			{
				pDocObjectItem->DoVerb(OLEIVERB_SHOW, pView);
			}
		}
	}</font></pre>

### <a name="MTS_0"></a>Microsoft Transaction Server Issues

**Feature Only in Enterprise Edition** The Microsoft Transaction Server is supported only in the Visual C++ Enterprise Edition.

#### <a name="MTS_1"></a>Read Microsoft Transaction Server (MTS) Readme

After installing Microsoft Transaction Server, please consult the Microsoft Transaction Server readme file, located in the \docs subdirectory of the Microsoft Transaction Server installation. The file contains information required to install, configure and run program components. The readme also contains descriptions of several useful samples and includes a list of known problems.

#### <a name="MTS_2"></a>MTS Objects Created with the ATL AppWizard Require Manual Running MTXRereg.Exe

After creating an MTS object using the ATL AppWizard, the custom build step to register the MTS object with MTS is unreliable. The workaround is either to call MTXRereg.Exe on the object manually, or to modify the custom build rule to point to MTXRereg.Exe explicitly in a specific directory. This is a known issue, and will be addressed for the final release.

#### <a name="MTS_3"></a>Disable Transaction Time Out While Debugging

Microsoft Transaction Server uses a time-out mechanism to keep components from deadlocking the system. If the transaction time-out is enabled while you are debugging the component, the transaction context may be destroyed, causing a protection fault. For example, stopping at a breakpoint and single stepping may exceed the time-out parameter.

To avoid this, you can disable this time-out from the Microsoft Transaction Server Explorer. Select the My Computer icon and select its properties. Under the **Options** tab on the **Properties** dialog box, you will see a transaction time-out section. To disable the time-out, set its value to 0\.

#### <a name="MTS_4"></a>No Proxy/Stubs with Dual Interfaces

The Microsoft Transaction Server is not capable of inheriting interfaces. The usual example of this is dual interfaces. Dual interfaces inherit from the **IDispatch** interface. If you create a Microsoft Transaction Server component that uses dual interfaces, you must use type libraries to contain the interface information. If you build a proxy/stub marshaling .dll for your dual interface component, you will get errors from Microsoft Transaction Server. See the Microsoft Transaction Server Readme for more information.

#### <a name="MTS_5"></a>Older Versions of MSDTC May Cause MTS Transaction Failures

MSDTC version 1.0, which shipped with SQL Server 6.5, has some resource leaks that may cause MTS transactions failures within an application. To determine whether a transaction is failing due to the MSDTC, look at the event viewer on the database server. If there is the following MSDTC application error: "Debug string message: ERROR: OUT OF RESOURCES IN SSTATE_UP," shut down the MSDTC, and restart. This will make available resources that MSDTC failed to release. The MSDTC that contains the fix is shipped in MTS 2.0 and NT4.0 SP4\. Alternatively, the fixed MSDTC can be picked up on the Microsoft Web Site [http://www.microsoft.com/com/mtsdb2-f.htm](http://www.microsoft.com/com/mtsdb2-f.htm).

### <a name="Data_Tools"></a>Microsoft Visual Database Tools

**Note**   The Microsoft Visual Database Tools are supported only in the Visual C++ Enterprise Edition. For issues specific to the Microsoft<sup>®</sup> Visual Database Tools™ installed with Visual C++ Enterprise Edition, see the [Visual Database Tools Readme](ReadmeDT.htm).

#### <a name="Data_Tools_2">DataView "Create New Extended Stored Procedure" Dialog Box Truncates Path of DLL Name</a>

If you create an extended stored procedure using DataView, and enter a very long path for the DLL name, the DLL name might be truncated (upon reopening the extended stored procedure). Because the name and path of the xp has been truncated, calls to this xp will fail.

##### Workaround

If you place the xproc in the binn directory of your local SQL Server installation (MSSQL\binn for SQL 6.5 or MSSQL7\binn for SQL 7.0), you do not need to specify a path for it.

#### <a name="Data_Tools_3">Visual C++ 6.0 Professional Edition Includes Read-Only Microsoft Database Tools</a>

Visual C++ 6.0 Professional Edition now includes the Microsoft Database Tools. Previously these tools shipped only with the Enterprise Edition.

The Professional Edition includes a read-only version of the Microsoft Database Tools. The read-only version allows you to view and modify tabular data. It does not allow you to modify database objects such as tables, diagrams, views, or stored procedures. The version of Microsoft Database Tools that ships with Visual C++ 6.0 Enterprise Edition allows full read/write capabilities.

#### <a name="Data_Tools_4">Jet Versions Supported by Visual C++</a>

The following table lists the Jet versions that Visual C++ supports:

<table width="90%" border="1">

<tbody>

<tr>

<td width="10%"><font size="2" face="Verdana">**Visual C++**</font></td>

<td width="10%"><font size="2" face="Verdana">**DAO**</font></td>

<td width="10%"><font size="2" face="Verdana">**Jet**</font></td>

<td width="10%"><font size="2" face="Verdana">**Office**</font></td>

</tr>

<tr>

<td width="10%"><font size="2" face="Verdana">4.x</font></td>

<td width="10%"><font size="2" face="Verdana">3.0</font></td>

<td width="10%"><font size="2" face="Verdana">3.0</font></td>

<td width="10%"><font size="2" face="Verdana">95</font></td>

</tr>

<tr>

<td width="10%"><font size="2" face="Verdana">5.0</font></td>

<td width="10%"><font size="2" face="Verdana">3.5</font></td>

<td width="10%"><font size="2" face="Verdana">3.5</font></td>

<td width="10%"><font size="2" face="Verdana">97</font></td>

</tr>

<tr>

<td width="10%"><font size="2" face="Verdana">6.0</font></td>

<td width="10%"><font size="2" face="Verdana">3.5</font></td>

<td width="10%"><font size="2" face="Verdana">3.6</font></td>

<td width="10%"><font size="2" face="Verdana">97</font></td>

</tr>

</tbody>

</table>

### <a name="Sample_Program_Issues_0"></a>Sample Program Issues

Samples are available on the MSDN CD-ROM in the \Samples\VC98 directory.

#### <a name="Sample_Program_Issues_3"></a>Ignore SFL Directory in Samples

Do not read or modify any of the files in the \SFL (Sample File List) directory in the Samples path. SFL does not contain Samples, documentation, or any other useful information, but the files it contains are required for Visual C++ documentation to work properly.

#### <a name="Sample_Program_Issues_16"></a>MINIMAL Sample Needs Modification to Build

You need to define _ATL_NO_UUIDOF in order to make Minimal.dsp build. This definition should be explained in the documentation for the ATL MINIMAL Sample as well. Also remove the _ATL_MIN_CRT define for Unicode Debug build.

#### <a name="Sample_Program_Issues_18"></a>COMMAP: Remove Mktyplib Compat Mode for MIDL

You need to remove the Mktyplib compat mode for MIDL in aggreg.dsp in the COMMAP sample.

#### <a name="Sample_Program_Issues_20"></a>AtlTangram: Needs Additional Files in Include Path

The AtlTangram Sample needs to have additional files specified in its include path:

<pre> <font size="2" face="Verdana">include=%include%;\samples\atl\atltangram;
			  \samples\atl\atltangram\atlgdiworld;
			  \samples\atl\atltangram\atlglworld;
			  \samples\atl\atltangram\atlmodel;
			  \samples\atl\atltangram\atlmodelps;
			  \samples\atl\atl\atltangram\atltangramcanvas;</font> </pre>

Also, in the same sample, the .lib file in AtlModelps.mak needs to link to msvcrt.lib

#### <a name="Sample_Program_Issues_21"></a>Some Samples Have SourceSafe Linkage

Some samples have SourceSafe linkage, which is safe to ignore.

#### <a name="Sample_Program_Issues_22"></a>DBVList

The DBVList sample files are available at \Samples\VC98\MFC\General\DBVList on the MSDN CD-ROM.

In the DBVList sample, debug UNICODE gets this error:

> <font size="2" face="Courier">DBVListSet.cpp(78) : error C2664: 'void __cdecl CString::Format(const unsigned short *,...)' : cannot convert parameter 1 from 'char [18]' to 'const unsigned short *'</font>

Also, you need to copy emp_all.mdb from \Samples\VC98\MFC\General\DBVList to the directory at which dbvlist.exe is located, or the **Fetch Results** button will not work.

#### <a name="Sample_Program_Issues_24"></a>ComplexDB

In the ComplexDB sample, you need to remove UUID.LIB from the link options. The ComplexDB files are available at \Samples\VC98\VcOleDb\Consumer\ComplexDB on the MSDN CD-ROM.

#### <a name="Sample_Program_Issues_25"></a>ATLMTO Sample Needs to Have ATL_MIN_CRT Turned Off

The ATLMTO sample (available in the VcOleDb\provider\atlmto directory) builds indicated below will currently not compile with the build set to MinDependency (causes a linker error (LNK2001) for **_main**). To build ATLMTO, you must turn off ATL_MIN_CRT.

*   Win32 Release MinSize
*   Win32 Release MinDependency
*   Win32 Unicode Release MinSize
*   Win32 Unicode Release Mindependency
*   Win32 Unicode Debug Minimal

NOTE: If you encounter this error message when using the ATLMTO OLE DB Provider:

<pre> <font face="Courier">ICommand->Execute FAILED!</font></pre>

You may have registered the Provider DLLs incorrectly. You must first register AtlMto.dll, then TestMto.dll.

#### <a name="Sample_Program_Issues_26"></a>Addendum to ComplexDB Sample Abstract

You need the Microsoft Data Access SDK to use the ComplexDB sample. The documentation for ComplexDB describes that it needs to connect to a DSN=OLE_DB_NWIND_Jet. The Microsoft Data Access SDK Setup adds this entry to the ODBC32 control panel; however, there is no database connected to it. You must manually edit this entry and select NWind.mdb.

#### <a name="Sample_Program_Issues_27"></a>ACCSPICT Sample Command Line Error

Win32 Release gets the /ZI and /O2 command line errors. To correct this problem, change the **Debug Info** in the **C++** tab of the **Project Settings** dialog from **Program Database for Edit and Continue** to **Program Database**.

#### <a name="Sample_Program_Issues_28"></a>CIRC and STOCKTICKERATL Samples Get MIDL Error

The CIRC sample gets the MIDL error:

> <font face="Courier">D:\samples\atl\circ\circ.idl(16) : error MIDL2270 : duplicate UUID. Same as : OLE_COLOR [ Type 'OLE_COLOR' ( Interface '__MIDL_itf_circ_0000' ) ]</font>

The STOCKTICKERATL sample gets the MIDL error:

> <font face="Courier">stocktickerATL.idl(15) : error MIDL2270 : duplicate UUID. Same as : OLE_COLOR [ Type 'OLE_COLOR' ( Interface '__MIDL_itf_stocktickerATL_0000' ) ]</font>

To correct this problem, remove the following line from the .idl file:

> <font face="Courier">typedef [uuid(66504301-BE0F-101A-8BBB-00AA00300CAB), public] DWORD OLE_COLOR;</font>

#### <a name="Sample_Program_Issues_29"></a>CIRCPROPS Sample Cannot Open circ.h Because of CIRC Problem

The CIRCPROPS sample cannot open circ.h because of the MIDL error in CIRC described [above](#Sample_Program_Issues_28). You get the following error:

> <font face="Courier">D:\samples\atl\circ\circProps.h(17) : fatal error C1083: Cannot open include file: 'circ.h': No such file or directory</font>

#### <a name="Sample_Program_Issues_30"></a>AUTODRIVE Gets Command Line Error

Win32 (80x86) Unicode Release gets the command line error "Command line error D2016 : '/ZI' and '/O2' command-line options are incompatible." To correct this, change the **Debug Info**, in the **C++** tab of the **Project Settings** dialog, from **Program Database for Edit and Continue** to **Program Database**.

#### <a name="Sample_Program_Issues_31"></a>Ignore SourceSafe Dialog When Loading ActiveDoc and Polygon ATL Samples

When you load the ActiveDoc or Polygon ATL samples, you will see a Visual SourceSafe dialog box, prompting you to search for the project. You can click No.

#### <a name="Sample_Program_Issues_32"></a>Rebuild All on SDK's INOLE2 Samples Will Give Linker Error

While doing a rebuild all of the SDK\COM\INOLE2 samples you might get the following errors:

<pre><font size="2" face="Courier">Creating library cosmo01.lib and object cosmo01.exp
polywin.obj : fatal error LNK1211: precompiled type information not found;
"precomp.obj" not linked or overwritten</font></pre>

This is because doing a rebuild all from the IDE does an nmake -a, which is not exactly the same as a plain nmake on a clean copy of the sample.

To fix the issue you will need to del *.pch in the sample directory, then Build (F7).

#### <a name="Sample_Program_Issues_33"></a>Workspace Files for the VCCOM COMMAP Sample Have Mismatched Targets

The workspace (.DSW) files for the VCCOM COMMAP sample have mismatched targets. Aggreg\aggreg.dsw targets Win32 Debug, and commap.dsw targets Win32 Unicode Debug. This is not a problem for builds done under NT, but it breaks the sample for builds done under Win95\. Changing either target to match the other fixes the problem.

#### <a name="Sample_Program_Issues_34"></a>Known Problems in MYPROV Sample

If you try to run the MYPROV sample under a free threaded client, you may encounter difficulty. To fix this problem, open the MyProviderDS.H file and look for the constructor for the CMyProviderSource class. Remove the CoInitialize and CoUninitialize statements and recompile. These lines of code are not emitted by the OLE DB Provider Wizard in ATL Object Wizard and are unique to this sample.

#### <a name="Sample_Program_Issues_35"></a>ActiveDoc ATL Sample Defaults to Unicode

The ActiveDoc ATL sample defaults to the Debug Unicode configuration. The DLL fails to register with no indication of error. Changing the active project to Win32 Debug fixes the problem.

### <a name="OLE_DB_0"></a>OLE DB Issues

#### <a name="OLE_DB_2.1">OLE DB Consumer Templates Samples</a>

<a name="OLE_DB_2.1">

The OLE DB Consumer Templates samples CatDB and DBViewer are located in the \Samples\VC98 directory on the MSDN CD-ROM.

**Note   **The DBViewer sample must be built with the /GZ compiler switch set. Otherwise, the application might draw a debug heap assertion on shutdown after calling stored procedures in SQL Server.

</a>

#### <a name="OLE_DB_2.1"></a><a name="OLE_DB_2.2">OLE DB Provider Templates Sample</a>

The OLE DB Provider Templates sample, Provider, is available in the \Samples\VC98\vcoledb\provider\provider directory on the MSDN CD-ROM. The sample demonstrates a basic single rowset provider. It mirrors what the OLE DB Provider Wizard generates when you create a default project.

The important class in the sample is the **CMyCommandHelper** class. It contains the methods for **GetData** and **Execute**. It also contains a PROVIDER_COLUMN_MAP that determines what data will be returned to the user when requesting a rowset. For more information on each of the base classes, consult the online documentation for OLE DB provider templates in the _Microsoft Foundation Class Library and Templates_.

#### OLE DB Provider Object in ATL Object Wizard

OLE DB Provider Templates help to implement the OLE DB data access interfaces. OLE DB can present any data source that is in a tabular format. OLE DB Provider Templates make the high performance OLE DB technology much easier to expose, and set the baseline for OLE DB providers.

AppWizard support is available to generate the framework for a standard provider. To utilize this functionality:

1.  Create an ATL COM project (DLL or EXE).
2.  Insert a new ATL Object. From the **Insert** menu or from **ClassView**, select **New ATL Object**.
3.  From the ATL Object Wizard, select **Data Access**, then **OLE DB Provider**.

#### <a name="OLE_DB_4"></a>Remove UUID2.lib from Link Line of OLE DB SDK TableCopy Sample

The TableCopy sample in the OLE DB SDK 1.1 will not compile correctly with Visual C++ 6.0\. You will receive a link error stating that UUID2.lib is not found. This is because UUID.lib, UUID2.lib, and UUID3.lib have been combined in the UUID.lib file in Visual C++ 6.0\. To fix the build problem, go to the **Project Settings** dialog box (**Project** menu) for the sample, select the **Link** tab, select **All configurations**, and remove the UUID2.lib entry from the **Object/Library Modules** line. You should then be able to successfully compile and link this sample.

#### <a name="OLE_DB_5"></a>TableCopy Faults with Oracle Data Connections

The TableCopy sample will not function correctly with an Oracle Data Connection. Select a different Data Connection type to use this sample.

#### <a name="OLE_DB_6"></a>Configuring OLE_DB_xx Data Sources in the ODBC Administrator

The OLE DB SDK installs Data Source Names with default paths, but depending upon your configuration, you may need to modify these Data Source Names using the ODBC Administrator to run properly on your machine. For more information, please refer to the OLE DB SDK documentation.

##### OLE_DB_NWind_Jet

1.  In Control Panel, double-click ODBC.
2.  Select the OLE_DB_NWind_Jet data source name, and click the **Configure** button.
3.  Navigate to the correct location in the OLE DB SDK subdirectory of the NWind.mdb file, and highlight it.
4.  Click **OK** to accept the file, then **OK** twice more to exit the Administrator.

##### OLE_DB_NWind_SQL

1.  In Control Panel, double-click ODBC.
2.  Select the OLE_DB_NWind_Jet data source name, and click the **Configure** button.
3.  Enter a server name that has the SQL Server Pubs database.
4.  Click the **Options>>** button and enter "pubs" for the database.
5.  Click **OK** to accept the info, then **OK** once more to exit the Administrator.

#### <a name="OLE_DB_9"></a>Binding Multiple Complex Databound Controls to the Same ADO Data Source Will Crash Application on Exit

If binding any pair of the following controls: DataList, DataCombo, or Hierarchical Flex Grid, to the same ADO Data Source control, the resulting compiled application will crash upon exiting. However, the dialog box will behave properly during test mode in the Resource editor. Other scenarios, such as binding a single control to an ADO Data Source or binding a simple databound control such as Masked Edit or Rich Text with a complex databound control also work properly.

#### <a name="OLE_DB_10"></a>Some Controls Do Not Draw Correctly in the Resource Editor

The DataGrid and DateTimePicker databound controls are unable to draw their hosting window in the Resource editor. As a result, these controls will appear incompletely drawn in design mode. However, there is no impact during run time, and the controls appear correctly in test mode and while executing.

#### <a name="OLE_DB_11"></a>Binding ADODC to Controls then Editing Record Source Will Draw Spurious Errors

If a control is bound to ADODC before the record source has been set in the ADODC, editing the record source will draw a series of spurious errors as you enter characters.

##### Workaround

Set the record source property in ADODC _before_ binding controls. This is a known issue and will be addressed in a future release.

#### <a name="OLE_DB_12"></a>Hierarchical Flex Grid Does Not Refresh on Second Query

If you bind the Hierarchical Flex Grid to an ADODC, and attempt to update the record source property of the ADODC programmatically, any subsequent reset will fail.

##### Workaround

Set the DataGrid control instead. This is a known issue and will be addressed in a future release.

#### <a name="OLE_DB_14.1"></a>Porting Providers Created with Visual C++ Technology Preview Release to Version 6.0

If you created OLE DB Providers with the Visual C++ Technology Preview release, they will not compile under the current version of Visual C++ 6.0\. To port them to the current version, look at the new Provider sample and note the changes to the various files. The following is a description of the changes and a guide to the new samples:

*   The **CommandHelper** and base classes no longer exist. The functionality has moved from this helper class to both the user's rowset and command classes. In addition, a class termed the User Record class has been introduced. The User Record class contains both the storage and **PROVIDER_COLUMN_MAP** or **GetColumnInfo** override. The **Rowset** class then templatizes on the **UserRecord**.
*   The **CommandHelper Execute** function has moved to the user's **CRowsetImpl** derived class. Note that the signature of the function remains the same.
*   The class **IATLCreatorImpl** no longer exists. It was replaced by **IObjectWithSiteImpl**. Simply replace all occurrences of **IATLCreatorImpl** with **IObjectWithSiteImpl** and **IATLCreator** with **IObjectWithSite**.
*   The **BEGIN_PROVIDER_COLUMN_MAP** now takes the name of the class in which it is contained.
*   **PROVIDER_COLUMN_ENTRY** is the only macro required and it automatically determines the appropriate type for both the **DBTYPE** and length. You need only supply the column name, ordinal, and field.
*   The **PROPSET** map is greatly simplified. **BEGIN_PROPSET_MAP** only needs the class in which the map is contained. **BEGIN_PROPERTY_SET** only requires the **PropertySet** GUID. **PROPERTY_INFO_ENTRY** only requires one parameter. The first parameter in the old **MACRO** def is the same as the new, so simply delete all but the first parameter.
*   The **InitXXSupported** functions are no longer needed or supported in the new templates. There is now a virtual in **CUtlProps::InitUPropSetsSupported**.
*   The guids file that was generated for you is not needed and will result in multiple link errors. Delete the guids file from the project.

#### <a name="OLE_DB_14.2"></a>Porting Consumers with Visual C++ Technology Preview Release to Version 6.0

See the document "OLE DB Consumer Template Changes Technology Preview to VC 6.0" in Knowledge Base article number Q187376.

#### <a name="OLE_DB_15"></a>Cannot Use ADO Databound Controls with Remote Data Source Control (MSRDC), or RDO Databound Controls with ADO Data Source Control (ADODC)

Visual C++ 6.0 provides a new set of databound controls based on ADO, a COM wrapper for OLE DB; it also provides a new data source control (ADODC).

However, Visual C++ 6.0 does not allow you to use the (new) ADO databound controls with the (old) remote data source control (MSRDC), or the (old) remote databound controls with the (new) ADO data source control (ADODC). You must use RDO databound controls with the remote data source control (MSRDC) and ADO databound controls with the ADO data source control (ADODC).

The exception is for simple bound data controls, which may be used interchangeably with the MSRDC and ADODC. The simple bound controls include the MS Masked Edit control and the MS Rich Text control.

The topics "ADO Data-Bound Controls," "RDO Data-Bound Controls," and "ADO and RDO Data-Bound Controls" in the _Visual C++ Programmer's Guide_ identify which data-bound controls are ADO-based and which are RDO-based.

#### <a name="OLE_DB_16"></a>Known OLE DB Provider Problems with Visual C++ Wizards

A complete list of known OLE DB provider problems with Visual C++ Wizards is referenced in Knowledge Base article Q181890.

#### <a name="OLE_DB_17"></a>Notes on Running OLE DB Provider Conformance Tests

Running the OLE DB Conformance Tests with the ATL Provider Templates : Threading Issues By default, the OLE DB Provider Wizard in ATL Object Wizard generates code for the provider to run in an apartment model. If you attempt to run this code with the conformance tests, you will initially get failures. This is because LTM.EXE, the tool used to run the OLE DB Conformance Tests, defaults to free threaded. We made the conscious decision to default to apartment model for performance and ease-of-use.

To correct this problem you can either change LTM or change the provider:

<pre><font size="2" face="Verdana">To change LTM to run in apartment threaded mode:
1\.  From the LTM main menu, go to Tools | Options.
2\.  On the general tab, change the threading model from Free Threaded to Apartment Threaded</font></pre>

<pre><font size="2" face="Verdana">To change your provider to run in free threaded mode:
1\.  In your provider project, search for all instances of CComSingleThreadModel and replace it with CComMultiThreadModel (should be in your data source, session, and rowset headers).
2\.  In your .RGS file, change the threading model from Apartment to Both
3\.  Follow correct programming rules for free threaded programming (i.e. lock on writes).</font></pre>

#### <a name="OLE_DB_18"></a>Simple Bound ADO Databound Controls Must Be Associated with a Column

When binding Simple Bound ADO Databound controls to an ADODC datasource control, the DataField property must also be set to a valid field. Otherwise the compiled application will assert in a running Debug build. The assertion is simply marking that the control has been bound to a null column. If the app is compiled under Release, the assert will no longer be there. Simple bound controls include the RichText, MaskedEdit, MonthView, Calendar, and DateTimePicker ActiveX controls.

#### <a name="OLE_DB_19"></a>Some OLE DB Providers Do Not Support Table Names with Spaces

The following OLE DB providers, which you can specify when using AppWizard to create an MFC EXE application, cannot compile and run when you specify a table name that contains a space:

*   OLE DB Provider for SQL Server
*   OLE DB Provider for Oracle
*   OLE DB Provider for ODBC to SQL Server
*   OLE DB Provider for ODBC to Oracle
*   User-defined custom provider

### <a name="SQL_0"></a>SQL and SQL Debugging

**Feature Only in Enterprise Edition** SQL and SQL debugging are supported only in Visual C++ Enterprise Editions.

#### <a name="SQL_1"></a>Data View and IDE Crashes When Opening Table Against DSN Using Oracle's ODBC Driver

If you want to create an Oracle 7.x ODBC data source, use the MS Oracle driver shipped with Visual C++. Visual C++ 6.0 currently does not work with Oracle 8.

#### <a name="SQL_2"></a>Previous Versions of Visual C++ Cannot Read SQL Diagrams Opened by Later Versions

Previous versions of Visual C++ cannot read SQL diagrams edited or opened by later versions. Specifically, if you create a database diagram connected to SQL Server 6.5 database in Visual C++ 5.0, then open the workspace in Visual C++ 6.0, you will not be able to reopen the workspace in Visual C++ 5.0\. You will get an error message that says: "The diagram cannot be opened since it was created with a newer version of the program."

#### **<a name="SQL_3"></a>Enabling SQL Debugging**

To enable SQL Debugging, you need to install the Visual C++ Enterprise Edition Server Components on your SQL Server machine. Before you run the setup program for the Visual C++ Server Components, you must first install the latest Service Pack for Windows NT, and the latest Service Pack for Microsoft SQL Server. Once these service packs are installed, you will be able to install the Visual C++ Server Components successfully. The setup program can be run directly from the \sqdbg_ss directory on CD-ROM 2.

#### <a name="SQL_4">Server-Side Setup Must Check SQL Server Account</a>

To enable debugging on your Microsoft SQL Server you must install the server-side components of this version of Visual Studio 6.0 on your SQL Server. You must also run Microsoft SQL Server under a valid user account and not under the "System Account". Under "System Account," SQL Server runs at a higher security level and cannot communicate with remote applications such as the Microsoft SQL Debugger.

To configure the SQL Server login account for SQL Debugging:

1.  Open Control Panel by clicking the **Start** button, **Settings**, then **Control Panel.**
2.  Double-click **Services,** select **MSSQLServer**, then click **Startup**.
3.  Select **This Account** and set the login ID to a valid user account and password.
4.  Click **OK** to close the dialog box and save your configuration.

**Note**   Any errors encountered while debugging the SQL Server will be listed in the event log. You can use this log to troubleshoot your debugging process.

#### <a name="SQL_5">SQL Server OLE DB Provider Requires New instcat.sql</a>

If you try to use the SQL Server OLE DB Provider, you must run the version of instcat.sql distributed with Microsoft Visual C++ 6.0 on SQL Server (version 6.5 and later). Instcat.sql is distributed with Visual C++ 6.0 and can be found in the \winnt\system32 directory upon installation.

If Instcat.sql is not run on your SQL Server, the provider is unable to retrieve metadata from the SQL Server. This breaks databinding, the MFC OLE DB Wizards, and OLE DB Templates.

#### <a name="SQL_6">MultiRead Provider Sample Needs Modification to Run</a>

In order for the MultiRead provider sample to compile, you must first remove oledb.lib from the link line, then remove the declaration for DBGUID_DEFAULT from stdafx.cpp. This is a known issue and will be addressed in a future release of Visual C++.

#### <a name="SQL_7">SQL Server OLE DB Provider Requires Indexes to be Set on Tables for IRowsetScroll</a>

When attempting to open an OLE DB rowset against SQL Server in which **IRowsetScroll** is used, all tables in the query must have an index set. Note that the MFC AppWizard automatically adds **IRowsetScroll** when generating an MFC application using OLE DB.

### <a name="Compiler_0"></a>Compiler, Linker, Debugger, and MIDL Compiler

#### <a name="Compiler_30"></a>New Debugger Features

##### Autoexp Variants, GUIDs

New rules have been added to the autoexp.dat file to display VARIANTs and GUIDs in more meaningful ways. They use the syntax $BUILTIN( type ). See autoexp.dat in the \Microsoft Visual Studio\Common\MSDEV98\bin directory for details.

##### VARIANT Display

Variants are automatically displayed in their correct form, so ints are displayed numerically, BSTRs as strings, and so on. Also displayed is the type of the variant, for example:

<pre> <font face="Courier">VARIANT vt;
	vt.vt = VT_I2;
	vt.iVal = 123</font> </pre>

<font face="Courier"><font face="Verdana">

vt will be displayed in Locals, Watch, and DataTips as {123 VT_I2}. VT_BYREF objects will also be displayed automatically, as will MFC's **COleVariants**.

##### GUID and IID Display

Types based on GUIDS (including IIDs, CLSIDs, and REFIIDs) are displayed by name (if found in the registry), or failing that, in the normal GUID hex form. Examples are {IID_IUnknown} or {1D2162240-1B7D-11CF-9D53-00AA003C9CB6}.

##### TIB

This is a new pseudo-register that displays the Thread Information Block (TIB, also confusingly known as a TEB) for the current thread. Like all registers, it may be prefixed with an @ sign. Information on the content of TIBs may be found in _Under the Hood_, _Microsoft Systems Journal (MSJ)_, May 96.

##### ERR

This is a new pseudo-register that displays the last error code for the current thread. It retrieves the same value as calling the **GetLastError** API. Like all registers, it may be prefixed with an @ sign.

If you use ERR in conjunction with the **,hr** modifier, the output displays the 32-bit error code with a comment, for example, "0x00000008 Not enough storage is available to process the command".

##### MMX Registers

You can now display MMX registers in the Watch and QuickWatch window using the symbols MM0-MM7\. MMX registers are 64-bit integer registers and will be displayed on all x86 machines, whether they support the MMX instructions or not.

##### V-Table & Function Pointer Display

Pointers to functions and v-table entries are now displayed symbolically wherever possible, including parameters, instead of being displayed simply as hex addresses (as they are in Visual C++ 5.0).

##### Disassembler Output

The disassembler output has been improved, particularly with regard to the inclusion of symbols in the output.

##### Undecorated Symbols

The Disassembler and Callstack windows now undecorate C++ names where they did not before, such as when displaying system callstacks from DBG files. For example, a function in RPCRT4.dll previously displayed as the somewhat meaningless ?MTAInvoke@@YGJPAUtagRPCOLEMESSAGE@@KPAUIRpcStubBuffer@@PAUIRpcChannelBuffer@@PAK@Z is now displayed as MTAInvoke with a proper argument list.

##### New Debugger Formatting Symbols

To use a formatting symbol, type the variable name, followed by a comma and the appropriate symbol. For example, if var has a value of 0x0065, and you want to see the value in character form, type var,c in the **Name** column of the Watch window. When you press ENTER, the character-format value appears:

<pre> <font face="Courier">var,c = 'e'</font> </pre>

<font face="Courier"><font face="Verdana">

For more information, search online (with **Search titles only** selected) for the topic "Symbols for Watch Variables" in the MSDN Library Visual Studio 6.0 documentation.

##### ,hr

This displays 32-bit results or error codes (HRESULTs or Win32 error codes) as common COM return values such as S_OK, E_NOTIMPL and so on. If that fails, it attempts to translate the error code into a comment.

Unfortunately it is not possible to set up an automatic rule in autoexp.dat to do this for types such as HRESULT; you must manually add the **,hr** postfix to symbol names in the Watch window.

##### ,st

This displays string values either as ANSI or Unicode, depending on the Unicode Strings setting, which is now used in the default autoexp.dat file to display MFC CStrings according to the current setting.

##### ,mq

This new formatting symbol displays memory as four quadwords, for example: 0x0012ffac 7ffdf00000000000 5f441a790012fdd4.

##### ,wm

This displays numeric values decoded into the names of windows message numbers (the **WM_** constants), so the following code:

<pre> <font face="Courier">WORD wMessage = WM_CLOSE
	wMessage,wm</font> </pre>

<font face="Courier"><font face="Verdana">

displays as **WM_CLOSE**.

##### ,wc

This displays numeric values decoded into window class flags (the **WC_** constants).

##### Load COFF & Exports

This new option allows additional debugging information to be loaded and can be found on the **Debug** tab (**Tools** menu, **Options** command). As this can affect debugger performance during program loading, the default for this option is off.

For more information, search online (with **Search titles only** selected) for the topic "The .dbg Files" in the _Visual C++ Programmer's Guide_ in the MSDN Library Visual Studio 6.0 documentation.

_COFF Symbols_

COFF symbols are used by other debuggers, but not by Visual C++ (which uses CodeView-format debug information), but sometimes it can be useful to read COFF info when no other is available. For example Visual Basic 5.01 includes a MSVBVM50.dbg file which supplies debug information in COFF format, so enabling this option allows that file to be read. To see what form of debug information is in a .dbg file, use dumpbin -headers and look at the Debug Directory for COFF.

_Exports_

When there is no other debugging information available (e.g. Windows 95 system files), then this option also converts the Export table of each loaded DLL into a symbol. To see what sort of symbols this will add for a particular DLL, use dumpbin -exports.

##### In-Process RPC Debugging

The debugger now supports debugging of in-process remote procedure calls (RPCs). You can find documentation for this feature in "Debugging COM Clients and Servers Using RPC" in the online documentation.

#### <a name="Compiler_37"></a>Some Linker Options Disable Edit and Continue

Whenever you see the following linker warning:

<pre> <font face="courier">LINK : warning LNK4075: ignoring /INCREMENTAL due to XXXX specification</font> </pre>

Edit and Continue support is simultaneously disabled in the linker, even if the project was compiled for Edit and Continue. Other options that disable incremental: adding /profile, changing the debug info type away from CV, /order, /release, or /force.

/opt:ref, /opt:icf, and /incremental:no will all produce a specific warning saying that Edit and Continue is disabled:

<pre> <font face="courier">LINK : warning LNK4075: ignoring /EDITANDCONTINUE due to /OPT specification</font> </pre>

Anything that disables producing a .pdb will also disable Edit and Continue, but without specific linker warnings.

#### <a name="Compiler_38"></a>Use New -opt:win98 Linker Switch if Targeting Windows 98 Platforms

If you build images intended to run on Windows 98, especially those that are redistributable, you should use the -opt linker switch with the win98 option. This allows the Windows 98 memory manager to cache executable images with a minimum of wasted space. This applies to x86 images only and is enabled with the following command to the linker:

<pre> <font size="2" face="Verdana">-opt:win98</font> </pre>

The Windows 9x memory manager does not cache portable executable images well because the file alignment (the value that is used to place the base of sections in the portable executable image) is 512 bytes by default. This works well for NT, in which the image file mapper, memory manager, and file cache are designed together. Win9x works altogether differently. The enhancements in Windows 98 only work when the sections in a portable executable image begin on a page boundary. The -opt:win98 switch performs the necessary file alignment.

When -opt:win98 and -opt:nowin98 are used, they are explicit and are always honored. Note that -opt:win98 is on by default. If you are building components that run only on NT, you should use -opt:nowin98.

This change does not impact Windows NT's or Windows 95's loading of images at all, nor does it impact the working set of the process in any way. The only impact is to the on-disk size. The average wasted space for 4096-byte file alignment can be characterized by the following expression:

<pre> <font size="2" face="Verdana">cbWasted = count-of-sections-in-image * 4096/2</font> </pre>

The average for the current 512-byte file alignment is:

<pre> <font size="2" face="Verdana">cbWasted = count-of-sections-in-image * 512/2</font> </pre>

The growth is therefore:

<pre> <font size="2" face="Verdana">cbGrowth = count-of-sections-in-image * (4096/2 - 512/2)
			= count-of-sections-in-image * 1792

	average count-of-bytes-Growth = count-of-sections-in-image * 1792 + 3584

	maximum count-of-bytes-Growth = count-of-sections-in-image * 4095 + 3584</font> </pre>

To get the count of sections, use dumpbin foo.exe. The summary will give you a list of sections in that image. Typically, you will see from 3 to 5 sections and you need to add one to that value, because it does not account for the portable executable header.

The only time you should not use -opt:win98 is when your portable executable image is very small to start with. Even if the image is slated for downloads, the wasted space is zero-filled and compresses very well.

#### <a name="Compiler_39"></a>Problem with Debugging COM/ActiveX Controls Through Internet Explorer 4.0 or Later

It is common to debug a COM/ActiveX control by embedding it in an HTML page, then loading the HTML page in a Web browser launched through the Visual C++ debugger. If you select **Settings** from the **Project** menu, and click on the **Debug** tab, you can designate the Web browser to use by typing its path in the **Executable for debug session** field, or by clicking the arrow button and selecting **Default Web browser**.

If the designated Web browser is Internet Explorer 4.0 or later, and if you have Internet Explorer's Active Desktop enabled, you may experience problems debugging your controls. With Active Desktop enabled, the Web browser that is launched through the debugger quickly terminates at the beginning of the debugging session, and the web browsing is turned over to the Internet Explorer process that is already running as your Active Desktop. Therefore, even if your control is running in the browser, the Visual C++ debugger has lost control of its execution because it is being executed in a different process than the one that was initially launched by the debugger.

##### Workaround

Add **/new** to the command line of Internet Explorer you designated in the **Debug** tab of the **Project Settings** dialog box. Or, within Internet Explorer, select **Internet Options** from the **View** menu. Click on the **Advanced** tab. Enable the option called **Browse in a new process**. This will prevent the Active Desktop from taking control of the browsing process when Internet Explorer is launched through the debugger.

#### <a name="Compiler_40"></a>STRICT Type Checking Is Enabled by Default

STRICT type checking is now defined by default. You should define NO_STRICT if you do not want to use STRICT type checking.

Note that the topic "Enabling STRICT Type Checking" in the _Visual C++ Programmer's Guide_ is [incorrect](#Doc_7).

#### <a name="Compiler_31"></a>Remote Debugging: Debug Monitor Password Field in MSVCMON.exe Disabled

Running MSVCMON.exe can potentially allow unauthorized access to the machine running MSVCMON.exe. Specifically, it may be possible for an unauthorized user to launch an application remotely on the target machine running MSVCMON.exe.

The Debug Monitor Password field in MSVCMON.exe has been disabled to reflect this behavior. You can still specify a password in the Visual Studio environment, but it will not be utilized by MSVCMON.exe.

Use caution when running MSVCMON.exe to enable remote debugging on a target machine.

#### <a name="Compiler_34"></a>_com_error Constructor Changed

The _com_error constructor, which takes an HRESULT and optional IErrorInfo interface pointer has changed, from:

<pre> <font face="courier">_com_error( HRESULT hr, IErrorInfo* perrinfo = NULL ) throw( );</font> </pre>

to:

<pre> <font face="courier">_com_error( HRESULT hr, IErrorInfo* perrinfo = NULL, bool fAddRef = false ) throw( );</font> </pre>

By default, the constructor will no longer call AddRef on a non-null IErrorInfo interface. This fixes a reference counting problem in the normal case where ownership of the interface is passed into the _com_error object, such as:

<pre> <font face="courier">throw _com_error(hr, perrinfo);</font> </pre>

If you do not wish your code to transfer ownership to the _com_error object, and the AddRef is required to offset the Release in _com_error's destructor, construct the object as follows:

<pre> <font face="courier">_com_error err(hr, perrinfo, true);</font> </pre>

#### <a name="Compiler_32"></a>Breakpoints Set in Some Circumstances Might Not Work

Breakpoints might not work if you set them in ActiveX controls that are hosted in IE4\. For information on how to work around this problem, search online (with **Search titles only** selected) for the topic "HOWTO: Debugging ActiveX Controls in IE 4.0 Browser" (Article ID Q167715) in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="Compiler_35"></a>Duplicate GUIDs Cause Build Failures Using uuid.lib

If you use uuid.lib in combination with other .lib files that define GUIDs (for example, oledb.lib and adsiid.lib), you might observe link error LNK2005 regarding duplicate definitions of some GUIDs. For example:

<pre> <font face="Courier">oledb.lib(oledb_i.obj) : error LNK2005: _IID_ITransactionObject
already defined in uuid.lib(go7.obj)</font> </pre>

##### Workaround

Add "/FORCE:MULTIPLE" to the linker command line options, and make sure that uuid.lib is the first library referenced.

#### <a name="Compiler_1"></a>Using Windbg with Visual C++ 6.0 Projects

Because of changes to the format of debugging information in Visual C++ 6.0, using the Windbg debugger (distributed in the Windows NT 4.0 Win32 SDK) to do source level debugging with Visual C++ 6.0 projects requires the following options:

Compile the project with:

<pre> <font face="courier">CL  /Z7  /c myapp.cpp</font> </pre>

Link the project with:

<pre> <font face="courier">LINK  /DEBUG  /PDB:NONE  myapp.obj</font> </pre>

You can then load myapp.exe in Windbg, step through your source code, and view the symbols in the Locals window.

#### <a name="Compiler_2"></a>_ATL_MIN_CRT and Link Error "unresolved external symbol _main"

When you build a Release version of an ATL project, you can get the following link error:

<pre> <font face="courier">LIBCMT.LIB(crt0.obj) : error LNK2001: unresolved external symbol _main</font> </pre>

This error occurs if you are using CRT functions that require CRT startup code. The Release configuration defines **_ATL_MIN_CRT**, which excludes CRT startup code from your EXE or DLL.

To avoid this error, do one of the following:

*   Remove **_ATL_MIN_CRT** from the list of preprocessor defines to allow CRT startup code to be included. On the **Project** menu, click **Settings**. In the **Settings For:** drop down list, choose **Multiple Configurations**. In the **Select project configuration(s) to modify** dialog box, click the check boxes for all Release versions, and then click **OK**. On the **C/C++** tab, choose the **General** category. Remove **_ATL_MIN_CRT** from the **Preprocessor definitions** edit box.
*   If possible, remove calls to CRT functions that require CRT startup code. Instead, use their Win32 equivalents. For example, use **lstrcmp** instead of **strcmp**. Known functions that require CRT startup code are some of the string and floating point functions.

#### <a name="Compiler_3"></a>DCOM95 Available for Distributed Applications

The Microsoft Distributed COM (DCOM) files for Windows 95 are useful for creating distributed applications. Some Visual C++ 6.0 samples require DCOM. You can find DCOM95 in the \dcom95 directory on the disc that includes "Microsoft Visual C++" on the label. (Disc 1 if you purchased Visual C++; Disc 3 if you purchased Visual Studio.) Check out the Visual C++ 6.0 Compiler COM support and Active Template Library ( ATL) with DCOM95\.

#### <a name="Compiler_11"></a>Debugging Windows API Functions with NT Symbols Loaded

If you have the NT symbols loaded and you want to debug Windows API functions, you need to enter the decorated name of the function with the name of the DLL in which the API resides when setting a breakpoint on the function. For example, if you want to set a breakpoint on the **MessageBeep** function, use the decorated name **{,,USER32.DLL}_MessageBeep@4**. The decorated name can be obtained in the map file created through linker options.

#### <a name="Compiler_12"></a>If Screen Flashes During Build or the Wrong Code Page Is Used When Debugging a Console Application

If you are using Windows 95, delete any of the following files from your computer:

*   _DEFAULT.pif
*   DEFAULT.pif
*   CONAGENT.pif

These files were used by Windows 3.x, and are not needed by Windows 95\. If they are used while you are debugging a console application, the country settings associated with the PIF files will be used, and could result in the wrong code page being loaded. A result of their use on Windows 95 may be screen flashing during a build, if you have specified console windows to be full screen.

#### <a name="Compiler_15"></a>MIDL2020: error generating type library: save all changes failed

This error can result if the path to the .idl file is longer than 126 characters. Oleaut32.dll does not currently support path names that are greater than 126 characters.

_Workaround:_

Reduce the path to the .idl file so that it is less than 126 characters.

#### <a name="Compiler_17"></a>Error Command Line Warning MIDL1009 : unknown argument ignored

MIDL.exe version 3.01.75 generates this error if its arguments are passed in a response file and one of the arguments is an MBCS-character file name that contains a space.

##### Workarounds

*   Use a batch file to invoke MIDL with its arguments.
*   Delete the space from the MBCS file name.

#### <a name="Compiler_41"></a>/Zn Option Obsolete

Because Visual C++ no longer does SBR packing, the /Zn option has no useful effect.

#### <a name="Compiler_42"></a>Delay Loading DLLs or Loading DLLs "on Demand"

Until Visual C++ 5.0, the only way to load a DLL "on demand" was by using the **LoadLibrary** and **GetProcAddress** Win32 APIs. If an application statically linked with a DLL there was no way to load a DLL "on demand." The operating system would load the DLL when the executable using it was loaded.

With Visual C++ 6.0, when statically linking with a DLL, the linker provides options to delay load DLLs until a program calls a function in a DLL.

An application can delay load a DLL using the /DELAYLOAD option of the Visual C++ 6.0 Linker with a helper function (default implementation provided by Visual C++ 6.0). The helper function will load the DLL "on demand" by calling the **LoadLibrary** and **GetProcAddress** APIs for you.

##### Example of Delay Loading a DLL

Here is a simple example of delay loading a DLL:

<pre>

 <font size="2" face="VERDANA">*   Start MSDEV and create a console application</font> 
*   <font size="2" face="VERDANA">Add t.cpp to the project:</font>

 <font face="Courier">//t.cpp
	#include <windows.h>
	//contains prototypes for helper function
	#include <delayimp.h> 
	//import library for helper function
	#pragma comment(lib, "delayimp")	
	void main()
	{
		// ...other code
	// USER32.DLL will load at this point
		MessageBox(NULL, "Hello", "Hello", MB_OK) ; 
		// ...other code
	}</font>

 <font size="2" face="VERDANA">*   In the **Project Settings** dialog box (**Project ** menu), select the **Linker** tab, and specify the following linker settings:
	/DELAYLOAD:USER32.dll 
The /DELAYLOAD option tells the linker to delay load the USER32.dll.
*   Build the DEBUG version of the project.  Step through the code using the debugger and you will notice that USER32.dll is loaded only when you make the call to the MessageBox API.</font> 

</pre>

##### Explicitly Unloading Delay-Loaded DLLs

To unload a delay-loaded DLL explicitly, use the /DELAY:UNLOAD linker option in conjunction with the **__FUnloadDelayLoadedDLL** function. For example:

<pre> <font face="Courier">#include <windows.h>
//contains prototypes for helper function
#include <delayimp.h>
#include "mydll.h"
//import library for helper function
#pragma comment(lib, "delayimp")	
#pragma comment(lib, "MyDLL")
void main()
{
	// ...other code
// MyDLL.DLL will load at this point
	MyDLLFunc() ; 
	//MyDLL.dll will unload at this point
	__FUnloadDelayLoadedDLL("MyDLL.dll") ;
		}</font> </pre>

Use the following linker settings with the above example:

<pre> <font face="Courier">/DELAYLOAD:MyDLL.dll /DELAY:UNLOAD</font> </pre>

Important notes on unloading a delay-loaded DLL:

*   The **__FUnloadDelayLoadedDLL** function is not documented. You can find the implementation in the file \VC\INCLUDE\DELAYIMP.CPP.
*   The name parameter of the **__FUnloadDelayLoadedDLL** function is case-sensitive. For example, "USER32.dll" works but "user32.dll" fails.
*   Comments associated with **__FUnloadDelayLoadedDLL** in DELAYIMP.CPP claims you can pass a NULL to unload all DLLs, but the results with a NULL parameter are unpredictable.

##### Binding Imports

The default linker behavior is to create a bindable Import Address Table for the delay-loaded DLL. If the DLL is bound, the helper function will attempt to use the bound information instead of calling **GetProcAddress** on each of the referenced imports. If either the timestamp or the preferred address do not match those of the loaded DLL, the helper function will assume the bound Import Address Table is out of date and will proceed as if the bound Import Address Table does not exist.

If you never intend to bind the DLL, specifying /DELAY:NOBIND on the linker's command line will prevent the bound Import Address Table from being generated.

#### <a name="Compiler_43"></a>NT System Symbol Setup Installs Debugging Files Only for the Language of Your Product

The NT System Symbol Setup (setupdgb.exe) installs the debugging (.dbg) files only for the particular language of your product. The debugging symbols corresponding to your operating system (if different) are available on your operating system retail CD-ROM.

#### <a name="Compiler_44"></a>New Dumpbin Option /LOADCONFIG

The **/LOADCONFIG** option of the dumpbin command dumps the **IMAGE_LOAD_CONFIG_DIRECTORY** structure pointed to by the optional header (Winnt.h).

#### <a name="Compiler_45"></a>New Compiler Switch /QIfist

This new compiler switch suppresses the call of the helper function, **_ftol**, when a conversion from a floating-point type to an integral type is required.

In addition to converting from a floating point type to integral type, the **_ftol** function ensures the rounding mode of the FPU is toward zero (truncate), by setting bits 10 and 11 of the control word. This guarantees that converting from a floating-point type to an integral type occurs as described by the ANSI C standard (the fractional portion of the number is discarded). When using the /QIfist switch, this guarantee no longer applies. The rounding mode will be one of four as documented in Intel reference manuals:

*   Round toward nearest (even number if equidistant)
*   Round toward negative infinity
*   Round toward positive infinity
*   Round toward zero

You can use the **_controlfp** C Run-Time function to modify the rounding behavior of the FPU. The default rounding mode of the CRT is "Round toward nearest." Using the /QIfist compiler switch can improve the performance of your application, but not without risk. You should thoroughly test the portions of your code that are sensitive to rounding modes before relying upon code built with /QIfist in production environments.

**Note**   This switch is not turned on by default because the rounding bits also affect FP to FP rounding (which occurs after every calculation), so when you set the flags for C-style (toward zero) rounding, your FP calculations might be different. This switch should not be used if your code depends upon the expected behavior of truncating the fractional portion of the floating-point number. If you are unsure, do not use this switch.

#### <a name="Compiler_46"></a>Cannot Debug Fibers on Windows 98

If you try to debug any application that uses fibers on Windows 98, the application will not behave the same way it behaves when run normally. When being debugged, the **SwitchToFiber** call will never switch to a fiber. This is a problem in kernel.dll and affects all user-mode debuggers including every version of Visual C++ and WinDbg. This problem does not occur on Windows NT. If you have to debug fiber code, or a component in an application that uses fibers, use Windows NT.

#### <a name="Compiler_47"></a>#pragma data_seg Affects Initialized Data Only

The **data_seg** pragma affects the placement of initialized data only. The **bss_seg** topic incorrectly states that **data_seg** works with initialized or uninitialized data.

#### <a name="Compiler_48"></a>Setting Breakpoints and Using Set Next Statement in Edited Code

If you edit code while debugging, you cannot set a breakpoint or the next statement in the new code until the code has been compiled. To compile code, either stop debugging and compile or use Edit and Continue (by choosing **Apply Code Changes** or any **Step** or **Go** command).

#### <a name="Compiler_49"></a>Using the /GX Option (Synchronous Exception Handling) with Command-Line Tools

The default for exception handling when using the command-line tools is /GX-, which explicitly turns off synchronous exception handling. When you create a project in the development environment, /GX is explicitly set for the project, and this overrides the command-line default. You can find this setting in the **Project Settings** dialog box (**Project** menu), on the **C/C++** tab, with the **C++ Language** category selected, in the **Enable exception handling** check box. If you clear this option, it does not display the command-line default, but it does use that default.

#### <a name="Compiler_50"></a>No F1 Help on TCP/IP Network Settings Dialog Box

The **TCP/IP Network Settings** dialog box (select **Debugger Remote Connection** from the **Build** menu), used for setting up remote debugging, has no F1 help available. If you need help using this dialog box, search online (with **Search titles only** selected) for the topic "Connecting the Host and Target Machines" in the MSDN Library Visual Studio 6.0 documentation."

#### <a name="Compiler_51"></a>Visual C++ 5.0 Can Read Version 6.0 Projects, but Behavior Is Undefined

Visual C++ 5.0 can read version 6.0 project (.dsp) files, but will not behave properly if you try to use these projects in Visual C++ 5.0\. (In fact crashes might occur.) If you find you need to use the version 6.0 project in version 5.0 after conversion, the version 5.0 .dsp file will be renamed with the extension ".001" so you can rename that file to .dsp. Note that the second time you convert the project, its extension is ".002" and it increments upon each conversion.

#### <a name="Compiler_52"></a>Windows NT Symbols Setup Gives Erroneous Message

Under Windows NT, when you select **Windows NT Symbols Setup** from the **Microsoft Visual C++ 6.0 Tools** menu, after entering the correct directory name in the source directory dialog box and selecting continue, you will receive an alert box with the message "Some of the symbol files could not be located in the input directory. Do you want to continue?" This alert will appear even though the directory has the correct files. If you select **Yes** on this alert, the symbols setup will proceed correctly.

#### <a name="Compiler_53"></a>AfxDumpStack Does Not Dump Readable Symbols from an MFC Application

If you issue the AfxDumpStack(AFX_STACK_DUMP_TARGET_DEFAULT) function from an MFC application and then run the debug version of the program in the debugger, you will see symbols such as:

<pre> <font size="2" face="Courier">5F43729C: WINNT\System32\MFC42D.DLL! Ordinal563 + 307 bytes</font></pre>

rather than a stack trace, which is what you would expect. This will be fixed in the next version of Visual C++.

#### <a name="Compiler_54"></a>Browsing Symbol Information Might Cause Access Violation in Projects where excel8.olb Has Been #imported

VC++ Browser (.bsc) files have an upper limit of 64K references per source module. If a source module exceeds this limit, Visual C++ might cause an access violation. Hitting the 64K limit is extremely rare, but is known to happen in the case of #importing excel8.olb. Some modules in this DLL surpass the 64K limit. When you #import excel8.olb, you generate excel8.tlh. Browsing for symbols in excel8.tlh can demonstrate the problem. To browse for symbols in VC++ from the editor, right mouse click on a symbol and select **Go To Definition** or **Go To Reference** from the context menu.

### <a name="VSS_0"></a>Visual SourceSafe Issues

The Visual C++ Enterprise Edition includes Visual SourceSafe. The Readme for Visual SourceSafe is [ReadmeSS.htm](ReadmeSS.htm).

#### <a name="VSS_1"></a>Converting a Visual C++ 4.x Project Directly from Source Control

Visual C++ no longer allows you to open a Visual C++ 4.x project from source control and convert it to the new project format from within Visual C++. Use the SourceSafe Explorer (or equivalent source control interface) to copy the files to a local hard disk, open the project in Visual C++ to do the conversion, and then check the files back into source control. After these steps, you may open the project out of source control as usual from Visual C++.

#### <a name="VSS_2"></a>Using Visual SourceSafe 5.0 with Keyword Expansion Requires Visual Studio 97 Service Pack 1

Without the updated Visual SourceSafe version from Visual Studio 97 Service Pack 1, the keyword expansion feature of Visual SourceSafe disables multiple-file actions for the **Check In** and **Add** commands. Using either of these commands with keyword expansion enabled causes Visual SourceSafe to operate on only one file and ignore the other files.

The requirement for SP1 applies only to the Visual Studio 5.0 **Source Control** commands under the **Project** menu, namely **Check In** and **Add to Source Control**. The requirement does not apply to stand-alone Visual SourceSafe.

This problem has been fixed in Visual SourceSafe 6.0.

### <a name="rmmscVisualComponentManager"></a>Visual Component Manager Issues

**<a name="rmmscKnownProblemsinVisualComponentManager"></a>The following are known problems with the Visual Component Manager:**

#### <a name="RelatedFilesTab"></a>"Related Files Tab (Component Properties Dialog Box)" topic incorrect

Visual Component Manager User Interface Reference: The topic "Related Files Tab (Component Properties Dialog Box)" incorrectly states that the tab is used to display and enter files that are related to the selected component. In fact, none of the information displayed on this tab can be modified. You can add related files to a component only when publishing or re-publishing the component. For more information, search online, with **Search titles only** selected, for "Publishing Components" in the MSDN Library Visual Studio 6.0 documentation.

#### <a name="RemovingRepository10RegistryKeys"></a>Removing Repository 1.0 Registry Keys

If you installed VCM 5.0 (previously available for web download) you will have the following Windows Registry keys setup. They were necessary for VCM 5.0 and the 1.0 version of the Repository. If you find the following Registry entries then it safe to remove them and may, in fact, improve VCM 6.0 performance.

*   HKEY_LOCAL_MACHINE\Software\Microsoft\Repository\CacheMaxAnnProps
*   HKEY_LOCAL_MACHINE\Software\Microsoft\Repository\CacheMaxObjects
*   HKEY_LOCAL_MACHINE\Software\Microsoft\Repository\CacheRelshipMaxCollections
*   HKEY_LOCAL_MACHINE\Software\Microsoft\Repository\CacheRelshipMaxRows
*   HKEY_LOCAL_MACHINE\Software\Microsoft\Repository\MaxRowCacheAge

#### <a name="AddingrepositorytablestoanexistingMDBfile"></a>Adding repository tables to an existing .mdb file

If you try to open an existing .mdb file from within VCM that is not a repository database (i.e., it does not contain the repository structure/tables), you will be asked if you want the repository tables added to the database. You should not do this for normal use; the repository should generally be in a separate database. This will work, but it can take as long as 10 minutes to create the repository structure in an existing .mdb file.

To create a brand new .mdb file containing the repository structure, right-click in the folder outline, click Repository, click New, and then enter the name of the file you want to create.
