---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 944835343e8187459021bb5a7f6e93b87c1e9b50
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081725"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/schema"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"respond-async" forHTTPHeaderField:@"Prefer"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchema *schema = [[MSGraphSchema alloc] init];
[schema setBaseType:@"microsoft.graph.externalItem"];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphProperty *properties = [[MSGraphProperty alloc] init];
[properties setName:@"ticketTitle"];
[properties setType: [MSGraphPropertyType String]];
[properties setIsSearchable:@"true"];
[properties setIsRetrievable:@"true"];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
[labelsList addObject: @"title"];
[properties setLabels:labelsList];
[propertiesList addObject: properties];
MSGraphProperty *properties = [[MSGraphProperty alloc] init];
[properties setName:@"priority"];
[properties setType: [MSGraphPropertyType String]];
[properties setIsQueryable:@"true"];
[properties setIsRetrievable:@"true"];
[properties setIsRefinable:@"true"];
[properties setIsSearchable:@"false"];
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