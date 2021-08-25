---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1ab8254f5a5041349561372234c67b52b3d892407d18895b83e7b652cec9e33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277637"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/id/contentTypes/id/associateWithHubSites"]]];
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