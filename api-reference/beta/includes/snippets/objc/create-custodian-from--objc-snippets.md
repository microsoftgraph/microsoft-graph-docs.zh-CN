---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2863a9dc835b8a4ea2e27e5092ecbd65468728b
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093591"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryCustodian *custodian = [[MSGraphEdiscoveryCustodian alloc] init];
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