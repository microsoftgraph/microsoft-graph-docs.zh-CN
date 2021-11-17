---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e15d246fc64e9be657321117ba027f6c1c3e83d1fb3da68a326ef505bb379d37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161383"
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