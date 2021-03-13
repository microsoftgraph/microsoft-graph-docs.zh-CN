---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39ae65574e45422831b5038a5628b8d750db7793
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773212"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/unifiedGroupSources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryUnifiedGroupSource *unifiedGroupSource = [[MSGraphEdiscoveryUnifiedGroupSource alloc] init];
[unifiedGroupSource setIncludedSources: [MSGraphEdiscoverySourceType mailbox]];

NSError *error;
NSData *unifiedGroupSourceData = [unifiedGroupSource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:unifiedGroupSourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```