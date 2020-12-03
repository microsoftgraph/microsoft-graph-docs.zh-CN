---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8dc91264e3c1704fc5d7f5d83d30c31349614f6f
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523558"
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