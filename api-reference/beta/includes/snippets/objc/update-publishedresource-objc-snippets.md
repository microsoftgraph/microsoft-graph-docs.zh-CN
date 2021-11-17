---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13ddf6d5ff84f575f70a1748be6fe9794cd1913e96b7d6c6222fb7bb331fbabd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163078"
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