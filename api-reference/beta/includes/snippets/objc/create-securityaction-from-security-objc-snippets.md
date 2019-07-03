---
description: 自动生成的文件。 不修改
ms.openlocfilehash: de0be8d93f8c90376e026b6e56c74c4b8bd4abe4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521518"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/securityActions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSecurityAction *securityAction = [[MSGraphSecurityAction alloc] init];
[securityAction setName:@"BlockIp"];
[securityAction setActionReason:@"Test"];
NSMutableArray *parametersList = [[NSMutableArray alloc] init];
MSGraphKeyValuePair *parameters = [[MSGraphKeyValuePair alloc] init];
[parameters setName:@"IP"];
[parameters setValue:@"1.2.3.4"];
[parametersList addObject: parameters];
[securityAction setParameters:parametersList];
MSGraphSecurityVendorInformation *vendorInformation = [[MSGraphSecurityVendorInformation alloc] init];
[vendorInformation setProvider:@"Windows Defender ATP"];
[vendorInformation setVendor:@"Microsoft"];
[securityAction setVendorInformation:vendorInformation];

NSError *error;
NSData *securityActionData = [securityAction getSerializedDataWithError:&error];
[urlRequest setHTTPBody:securityActionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```