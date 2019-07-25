---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dfc6877c7cd834a3526d4bdd8475ced575f15a58
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724953"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *filterOperatorSchemaList = [[NSMutableArray alloc] init];
        filterOperatorSchemaList = [jsonFinal valueForKey:@"value"];
        MSGraphFilterOperatorSchema *filterOperatorSchema = [[MSGraphFilterOperatorSchema alloc] initWithDictionary:[filterOperatorSchemaList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```