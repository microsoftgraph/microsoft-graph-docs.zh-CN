---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a3e449f0dc1cc06b1abbdeec06f4a1ff38f82847
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874990"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphPublishedResource *publishedResource = [[MSGraphPublishedResource alloc] init];
[publishedResource setDisplayName:@"Demo provisioning (updated)"];

NSError *error;
NSData *publishedResourceData = [publishedResource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:publishedResourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```