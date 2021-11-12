---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 518d8974452779dd0e427dd29b2e51928dc1eb06427f3ca832102fa3c843c255
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219553"
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