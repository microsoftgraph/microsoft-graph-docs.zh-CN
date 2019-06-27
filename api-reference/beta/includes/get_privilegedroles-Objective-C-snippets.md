---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8b93dda33b3011c18049426771d0cc1827de077
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330147"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedRoles"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *privilegedRoleList = [[NSMutableArray alloc] init];
        privilegedRoleList = [jsonFinal valueForKey:@"value"];
        MSGraphPrivilegedRole *privilegedRole = [[MSGraphPrivilegedRole alloc] initWithDictionary:[privilegedRoleList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```