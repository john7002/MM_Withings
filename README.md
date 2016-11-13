# MM_Withings module for MagicMirror

A simple MagicMirror module to collect data from Withings devices and display related information (weight, sleep, steps etc.).

![MM_Withings ](https://github.com/john7002/MM_Withings/blob/master/.ressources/module_preview.png)    

## How to use it?                                                                                                                                           

To use this module, you first need [MagicMirror](https://github.com/MichMich/MagicMirror) and a Withings account.

 -1) Create a folder MM_Withings in your module folder
-2) Then run : ' git clone https://github.com/john7002/MM_Withings '

### Configuration
Create a developer app from [Withings partner app](http://oauth.withings.com/partner/dashboard), you will get an API Key and an API Secret.
	
This api website from [Withings](http://oauth.withings.com/api) will help you to get additional informations regarding your Withings account (step1 to step3). Please note:
- oauth_signature
- oauth_token
- clientID
		
In you config/config.js file, declare the module:
```
{                                                                                                                                                   
  module: 'MM_Withings',                                                                                                                          
  position: 'top_left',                                                               
  config:{                                                                                                                                   
  oauth_consumer_key: '', // your API key app
  oauth_signature: '',//Withings API step3
  oauth_token:'',//Withings API step3
  clientID:''  // clientID from Withings API step 2   																                                       															                                                                              
  }                                                                                                                                           
}                
```
