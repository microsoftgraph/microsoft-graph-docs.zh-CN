---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b2f3299a0733167c1cdf67d7331eb10b9c23b4b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330093"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groupLifecyclePolicies/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroupLifecyclePolicy *groupLifecyclePolicy = [[MSGraphGroupLifecyclePolicy alloc] init];
[groupLifecyclePolicy setGroupLifetimeInDays: 180];
[groupLifecyclePolicy setManagedGroupTypes:@"Selected"];
[groupLifecyclePolicy setAlternateNotificationEmails:@"admin@contoso.com"];

NSError *error;
NSData *groupLifecyclePolicyData = [groupLifecyclePolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupLifecyclePolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```