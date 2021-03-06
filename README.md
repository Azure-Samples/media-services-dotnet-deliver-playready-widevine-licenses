---
page_type: sample
languages:
- csharp
products:
- azure
description: "Azure Media Services (AMS) enables you to ingest, encode, add content protection, and stream your content (see this article for details)."
urlFragment: media-services-dotnet-deliver-playready-widevine-licenses
---

# Use Azure Media Services v2 to deliver PlayReady and/or Widevine licenses with .NET

## NOTE
 
You can find the latest and most extensive Media Services v3 .NET samples in the [Azure Media Services v3](https://github.com/Azure-Samples/media-services-v3-dotnet) repository.

## Overview

Azure Media Services (AMS) enables you to ingest, encode, add content protection, and stream your content (see this article for details). However, there are customers who only want to use AMS to deliver licenses and/or keys and do encoding, encrypting and streaming using their on-premises servers. This samples shows how to configure AMS to deliver PlayReady and/or Widevine licenses.

For detailed information about the sample, see [Use AMS to deliver PlayReady and/or Widevine licenses or AES keys](http://azure.microsoft.com/documentation/articles/media-services-deliver-keys-and-licenses/).

## How To Run This Sample

To run this sample you will need:

- Visual Studio
- An Azure subscription
- Latest Azure Media Services .NET SDK (which will be installed when you re-build the project).

### Step 1:  Clone or download this repository

### Step 2: Update the app.config file

Update the appSettings section of the app.config file with appropriate values. For more information, see [this](https://docs.microsoft.com/azure/media-services/media-services-use-aad-auth-to-access-ams-api) topic.

	<appSettings>
		<add key="AMSAADTenantDomain" value="tenant"/>
		<add key="AMSRESTAPIEndpoint" value="endpoint"/>
		<add key="AMSClientId" value="id"/>
		<add key="AMSClientSecret" value="secret"/>

		<add key="Issuer" value="http://testacs.com" />
		<add key="Audience" value="urn:test" />
	</appSettings>
		  
### Step 3: Start a streaming endpoint

Make sure to start the streaming endpoint. For more information, see: [streaming endpoints](https://docs.microsoft.com/azure/media-services/media-services-portal-manage-streaming-endpoints).

### Step 4:  Run the sample

Clean the solution, rebuild the solution, and run it. 

## About the code

For more information, see  [Use AMS to deliver PlayReady and/or Widevine licenses or AES keys](http://azure.microsoft.com/documentation/articles/media-services-deliver-keys-and-licenses/).

## More information

You can view AMS learning paths here:

- [AMS Live Streaming Workflow](http://azure.microsoft.com/documentation/learning-paths/media-services-streaming-live/)
- [AMS on Demand Streaming Workflow](http://azure.microsoft.com/documentation/learning-paths/media-services-streaming-on-demand/)
