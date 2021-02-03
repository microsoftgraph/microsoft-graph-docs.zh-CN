---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ab2d19882d847166b5b970d948c8e0ba3421a51
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093608"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources"]]];
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