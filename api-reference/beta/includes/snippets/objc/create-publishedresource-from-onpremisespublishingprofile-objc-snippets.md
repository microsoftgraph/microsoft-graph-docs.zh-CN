---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6687849e54916269a4c26cec352a91172b2e6d70878c10eae3483b48e696c51e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163081"
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