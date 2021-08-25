---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0be8a05a27f99bbd835a798f8473648c282cd5bc
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516042"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/schema"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExternalConnectorsSchema *schema = [[MSGraphExternalConnectorsSchema alloc] init];
[schema setBaseType:@"microsoft.graph.externalItem"];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphExternalConnectorsProperty *properties = [[MSGraphExternalConnectorsProperty alloc] init];
[properties setName:@"ticketTitle"];
[properties setType: [MSGraphExternalConnectorsPropertyType string]];
[properties setIsSearchable:@"true"];
[properties setIsRetrievable:@"true"];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
[labelsList addObject: @"title"];
[properties setLabels:labelsList];
[propertiesList addObject: properties];
MSGraphExternalConnectorsProperty *properties = [[MSGraphExternalConnectorsProperty alloc] init];
[properties setName:@"priority"];
[properties setType: [MSGraphExternalConnectorsPropertyType string]];
[properties setIsQueryable:@"true"];
[properties setIsRetrievable:@"true"];
[properties setIsSearchable:@"false"];
[propertiesList addObject: properties];
MSGraphExternalConnectorsProperty *properties = [[MSGraphExternalConnectorsProperty alloc] init];
[properties setName:@"assignee"];
[properties setType: [MSGraphExternalConnectorsPropertyType string]];
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