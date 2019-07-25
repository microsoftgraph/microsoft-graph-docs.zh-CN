---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b35b57cad18bf30b7a2a09f4fea5704d2924c676
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875006"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/publishedResources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPublishedResource *publishedResource = [[MSGraphPublishedResource alloc] init];
[publishedResource setDisplayName:@"New provisioning"];
[publishedResource setResourceName:@"domain1.contoso.com"];

NSError *error;
NSData *publishedResourceData = [publishedResource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:publishedResourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```