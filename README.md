# Synchrophasor Application Tool
Operation Instructions : 
Please download the attached files WSCC 9 bus modified.PWB and WSCC 9 bus modified.pwd and the required software from Power World Dynamic Studio version 21 https://www.powerworld.com/gloveroverbyesarma.

In Dynamic Studio open the case and the oneline file and setup the server IP address and port.

Verify the instructions of C-compiler or similar and install it if needed. To check type "mex -setup" into MATLAB Command Window.
As the app is programmed for IEEE WSC 9-bus system ensure all the phasors are being parsed as per the same.

Installation :
After downloading the file. Set the current folder to the one having the app setup.
Then click on APPS-->>Install App.
Browse and select "SynchrophasorApp.mlappinstall" form the downloaded location.
After Intallation select "SynchrophasorApp" from MyApps to run the app.

In the synchrophasor application tool specify the IP address and other relevant parameters alongwith the lines for which power flow is to be calculated.

# Note : Select any two lines in active power tab, and two lines in reactive power tab.
Due to the fact that the application is cuurently under development.

In case of the following error:
  "
  Error using icinterface/fopen (line 83)
  Unsuccessful open : Connection refused: connect
  
  Error in ICT_initialisation (line 73)
      fopen(SADF>Connection_primary);
     
  Error in SADF_run (line 58)
  ICT_initialisation();
  
  Error in run (line 86)
  evalin('caller', [script ';']);
  "
Please verify the connection parameters in the settings tab of the SynchrophasorApp.
