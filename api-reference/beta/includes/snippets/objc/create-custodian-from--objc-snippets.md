---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 90586674eaaabec3f44dba05ebc79bda00b820b7
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659517"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCustodian *custodian = [[MSGraphCustodian alloc] init];
[custodian setEmail:@"AdeleV@contoso.com"];
[custodian setApplyHoldToSources:@"true"];

NSError *error;
NSData *custodianData = [custodian getSerializedDataWithError:&error];
[urlRequest setHTTPBody:custodianData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```