---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0543bea767c489fc4be6ad484fad4c4197d8458c
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013623"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/usageRights?$filter=state%20in%20('active',%20'suspended')%20and%20serviceIdentifier%20in%20('ABCD')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUsageRights *usageRights = [[MSGraphUsageRights alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```