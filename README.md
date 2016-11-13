# MM_Withings module for MagicMirror

A simple MagicMirror module to collect data from Withings devices and display related information (weight, sleep, steps etc.).

## How to use it?                                                                                                                                           

To use this module, you first need [MagicMirror](https://github.com/MichMich/MagicMirror) and a Withings account.

 -1) Create a folder MM_Withings in your module folder
	-2) Then run : git clone https://github.com/john7002/MM_Withings

### Configuration
Create a developer app from [Withings partner app](http://oauth.withings.com/partner/dashboard), you will obtain two keys:
	- API Key
	- API Secret
	
	This api website from [Withings](http://oauth.withings.com/api) will help you to get additional informations regarding your Withings account. Please note:
		- oauth_signature
		- oauth_token
		- clientID
		
		In you config/config.js file, declare the module:
```
{                                                                                                                                                   
        module: 'MM_Withings',                                                                                                                          
        position: 'top_left',                                                               
        config: {                                                                                                                                   
                oauth_consumer_key: '', // your API key app
        								oauth_signature: '', // generated from api Withings (step3).
																oauth_token:'',// token generated from api Withings (step3).
																clientID:''  // your clientID account received from api Withings site (step 2).                                                                         
        }                                                                                                                                           
}                
```

 
