---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03ed45bfbd0f202d3a4170a362bdc6ee23a7ec2e164b20abe693b94a6730366c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274173"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/387566cc-38ae-4e85-ab4b-cd2dd34faa07/userSources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryUserSource *userSource = [[MSGraphEdiscoveryUserSource alloc] init];
[userSource setEmail:@"adelev@contoso.com"];
[userSource setIncludedSources: [MSGraphEdiscoverySourceType mailbox]];

NSError *error;
NSData *userSourceData = [userSource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userSourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```