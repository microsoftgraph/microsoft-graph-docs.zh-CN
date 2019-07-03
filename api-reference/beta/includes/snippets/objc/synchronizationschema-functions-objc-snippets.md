---
description: 自动生成的文件。 不修改
ms.openlocfilehash: af36e764815ad84b05b84b320913897c46e99536
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478393"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *attributeMappingFunctionSchemaList = [[NSMutableArray alloc] init];
        attributeMappingFunctionSchemaList = [jsonFinal valueForKey:@"value"];
        MSGraphAttributeMappingFunctionSchema *attributeMappingFunctionSchema = [[MSGraphAttributeMappingFunctionSchema alloc] initWithDictionary:[attributeMappingFunctionSchemaList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```