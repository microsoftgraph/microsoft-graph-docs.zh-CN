---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46d28e3fccf913e030266aff1717a3b6cd7da5bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "60729414"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{siteId}/contentTypes/{contentTypeId}/associateWithHubSites"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *hubSiteUrlsList = [[NSMutableArray alloc] init];
[hubSiteUrlsList addObject: @"https://graph.microsoft.com/beta/sites/id"];
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