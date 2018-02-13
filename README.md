# Aspose.Storage for Cloud
[Aspose.Storage for Cloud](https://apireference.aspose.cloud/storage/) is a true REST API that that provides managers for multiple storage types.

Our Cloud SDKs are wrappers around REST API in various programming languages, allowing you to process documents in language of your choice quickly and easily, gaining all benefits of strong types and IDE highlights. This repository contains new generation SDKs for Aspose.Storage for Cloud and examples.

These SDKs are now fully supported. If you have any questions, see any bugs or have enhancement request, feel free to reach out to us at [Free Support Forums](https://forum.aspose.cloud/).
 
See [API Reference](https://apireference.aspose.cloud/storage/) for full API specification.

# Currently Available SDKs

The following SDKs are currently available:

Directory | Description
--------- | -----------
[.NET SDK](SDKs/NET) | Cloud SDK for .NET Framework 2.0 and higher

To use these SDKs, you will need App SID and App Key which can be looked up at [Aspose Cloud Dashboard](https://dashboard.aspose.cloud/#/apps) (free registration in Aspose Cloud is required for this).

# Comparison with Old generation SDKs
New SDKs have the following advantages over the [previous versions](https://github.com/aspose-total/Aspose.Total-for-Cloud/tree/master/SDKs/Aspose.Storage-Cloud-SDK-for-.NET):
+ Classes, methods and properties have comments and are IDE-friendly
+ Better security
+ Usage of Request/Response classes to represent long lists of parameters. This allows for cleaner code and easier backwards-compatibility going forward

New SDKs are not backwards compatible with previous generation because of the last item. It should be straightforward to convert your code to using Request/Response objects, if you need any help on migration please ask at [Free Support Forums](https://forum.aspose.cloud/).

## Getting Started

```csharp
using System;
using System.Diagnostics;
using Aspose.Storage.Cloud.Sdk.Api;
using Aspose.Storage.Cloud.Sdk.Model;
using Aspose.Storage.Cloud.Sdk.Model.Requests;

namespace Example
{
    public class Example
    {
        public void Main()
        {
            //TODO: Get your AppSID and AppKey at https://dashboard.aspose.cloud (free registration is required).
            var configuration = new Configuration
            {
                AppSid = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
                AppKey = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
            };

            var apiInstance = new FileApi(configuration);
	    try
	    {		
		    var request = new FileGetDownloadRequest();
		    request.path = "TestFile.pdf";
		    request.storage = "StorageName";
		    var response = FileApi.FileGetDownload(request);
	    }
	    catch(Exception ex)
	    {
	    	Debug.Print("Exception when calling FileApi.FileGetDownload: " + e.Message);
	    }
            

        }
    }
}
```

# Licensing
All Aspose.Storage for Cloud SDKs are licensed under [MIT License](LICENSE).

# Resources
+ [**Website**](https://www.aspose.cloud)
+ [**Product Home**](https://products.aspose.cloud/storage/cloud)
+ [**Documentation**](https://docs.aspose.cloud/display/storagecloud/Home)
+ [**Free Support Forum**](https://forum.aspose.cloud/c/storage)
+ [**Paid Support Helpdesk**](https://helpdesk.aspose.cloud/)
+ [**Blog**](https://blog.aspose.cloud/category/aspose-products/)
