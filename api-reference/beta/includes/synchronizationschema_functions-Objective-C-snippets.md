---
description: 自动生成的文件。 不修改
ms.openlocfilehash: af36e764815ad84b05b84b320913897c46e99536
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329876"
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