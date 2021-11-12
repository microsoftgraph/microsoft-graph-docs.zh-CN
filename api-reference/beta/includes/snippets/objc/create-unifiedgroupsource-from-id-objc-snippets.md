---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f7ec1c12da4e5b19ea1c23d156f7391fbb6a59b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60946258"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/custodians/8904528fef4d4578b44f71a80188f400/unifiedGroupSources"]]];
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