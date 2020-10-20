---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61fa32f93968ae41e76f7fd5c7403a2de9d86376
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611598"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/domains/contoso.com"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDomain *domain = [[MSGraphDomain alloc] init];
[domain setIsDefault: true];
NSMutableArray *supportedServicesList = [[NSMutableArray alloc] init];
[supportedServicesList addObject: @"Email"];
[supportedServicesList addObject: @"OfficeCommunicationsOnline"];
[domain setSupportedServices:supportedServicesList];

NSError *error;
NSData *domainData = [domain getSerializedDataWithError:&error];
[urlRequest setHTTPBody:domainData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```