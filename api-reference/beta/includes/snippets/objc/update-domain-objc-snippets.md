---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4b5b87aea530c96c05443f915d3eb1bbda7a28d9f4986e86048d0fa42c268d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104814"
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