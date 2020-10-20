---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de0be8d93f8c90376e026b6e56c74c4b8bd4abe4
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607640"
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