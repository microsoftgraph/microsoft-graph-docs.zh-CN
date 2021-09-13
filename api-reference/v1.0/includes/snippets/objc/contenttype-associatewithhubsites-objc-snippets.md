---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d4f39067f6e2c937263620a48680aca4d71ff5d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147666"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/contentTypes/{contentTypeId}/associateWithHubSites"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *hubSiteUrlsList = [[NSMutableArray alloc] init];
[hubSiteUrlsList addObject: @"https://graph.microsoft.com/v1.0/sites/{site-id}"];
payloadDictionary[@"hubSiteUrls"] = hubSiteUrlsList;

BOOL propagateToExistingLists = NO;
payloadDictionary[@"propagateToExistingLists"] = propagateToExistingLists;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```