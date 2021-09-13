---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0c075ae7d5a2a3f7a8264b8518b73b7f2cc15b9ece48c171776471c77165f5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409092"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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