---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a59336d1228547a85ee226e59b9b6392000ea937
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124148"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/tasks/lists/AAMkADliMmU5YjJlLTVmMmQtNGQzNS1iYjA0LTdmZTA2NTI0MTE5YwAuAAAAAADdOMUbUmCfTKa7OC-fqjkdAQBnu3olF7NfToRyJ2f__TNcAAAAAAESAAA=/tasks/AAkALgAAAAAAHYQDEapmEc2byACqAC-EWg0AZ7t6JRezX06Ecidn-vkzXAABPDii4gAA/linkedResources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphLinkedResource_v2 *linkedResource_v2 = [[MSGraphLinkedResource_v2 alloc] init];
[linkedResource_v2 setWebUrl:@"https://microsoft.com"];
[linkedResource_v2 setApplicationName:@"Microsoft"];
[linkedResource_v2 setDisplayName:@"Microsoft"];
[linkedResource_v2 setExternalId:@"dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"];

NSError *error;
NSData *linkedResource_v2Data = [linkedResource_v2 getSerializedDataWithError:&error];
[urlRequest setHTTPBody:linkedResource_v2Data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```