---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce3bfe6f4de6fb9393edbab159a8e54bbe30ff9fa6c8d3a1d796e54d289e0b19
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221289"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/deviceManagement/virtualEndpoint/deviceImages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCloudPcDeviceImage *cloudPcDeviceImage = [[MSGraphCloudPcDeviceImage alloc] init];
[cloudPcDeviceImage setDisplayName:@"Display Name value"];
[cloudPcDeviceImage setOsBuildNumber:@"OS Build Number value"];
[cloudPcDeviceImage setOperatingSystem:@"Operating System value"];
[cloudPcDeviceImage setVersion:@"Version value"];
[cloudPcDeviceImage setSourceImageResourceId:@"/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"];

NSError *error;
NSData *cloudPcDeviceImageData = [cloudPcDeviceImage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:cloudPcDeviceImageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```