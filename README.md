# AutoHotKey

This project is associated with an internship through Shepherd University and Fiserv Corporation.

The goal of this project is to update AutoHotKey macros used to automate account data manipulation from Web based systems. It will focus primarily on collecting data from Web pages to create documents using DOM functionality.

#NoEnv
#WinActivateForce
#SingleInstance Force
#Include %A_ScriptDir%
SetTitleMatchMode, 2
SetTitleMatchMode, Fast

MakeSureOpen()
{
  WinWait, http://google.com,
  If WinNotActive, http://google.com, ,WinActivate, http://google.com,
  WinWaitActive, http://google.com,
  Sleep, 200
  }
  
  Msgbox,3,Macro_Name, Description_Here `n and here
  IfMsgbox Cancel
  Goto GuiClose
  else IfMsgbox No
  {
  Goto Next_Step
  }
  else IfMsgbox Yes
  ;;;code
  return
  Next_Step:
  ;;;code
  return
  GuiClose:
  #=::ExitApp  
  
  
