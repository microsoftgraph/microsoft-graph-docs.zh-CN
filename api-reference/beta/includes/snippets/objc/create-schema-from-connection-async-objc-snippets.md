---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b3183b1bd128cc50892a5c788347945cd2d6424
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995480"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/connections/contosohr/schema"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"respond-async" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchema *schema = [[MSGraphSchema alloc] init];
[schema setBaseType:@"microsoft.graph.externalItem"];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphProperty *properties = [[MSGraphProperty alloc] init];
[properties setName:@"title"];
[properties setType: [MSGraphPropertyType String]];
[properties setIsSearchable:@"true"];
[properties setIsRetrievable:@"true"];
[propertiesList addObject: properties];
MSGraphProperty *properties = [[MSGraphProperty alloc] init];
[properties setName:@"priority"];
[properties setType: [MSGraphPropertyType String]];
[properties setIsQueryable:@"true"];
[properties setIsRetrievable:@"true"];
[propertiesList addObject: properties];
MSGraphProperty *properties = [[MSGraphProperty alloc] init];
[properties setName:@"assignee"];
[properties setType: [MSGraphPropertyType String]];
[properties setIsRetrievable:@"true"];
[propertiesList addObject: properties];
[schema setProperties:propertiesList];

NSError *error;
NSData *schemaData = [schema getSerializedDataWithError:&error];
[urlRequest setHTTPBody:schemaData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```