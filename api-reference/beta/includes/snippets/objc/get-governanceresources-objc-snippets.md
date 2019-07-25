---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2acb36a754fcea094b50f146dba5ec9f77a49cc1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713928"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/resources"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *governanceResourceList = [[NSMutableArray alloc] init];
        governanceResourceList = [jsonFinal valueForKey:@"value"];
        MSGraphGovernanceResource *governanceResource = [[MSGraphGovernanceResource alloc] initWithDictionary:[governanceResourceList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```