---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 652b22341a8eeb82e70781579f54a99666b41616
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725334"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/delta"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *servicePrincipalList = [[NSMutableArray alloc] init];
        servicePrincipalList = [jsonFinal valueForKey:@"value"];
        MSGraphServicePrincipal *servicePrincipal = [[MSGraphServicePrincipal alloc] initWithDictionary:[servicePrincipalList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```