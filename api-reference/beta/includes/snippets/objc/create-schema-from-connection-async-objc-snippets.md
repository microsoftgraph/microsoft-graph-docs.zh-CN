---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb07da4ed8b7238923b92a86e76bfd9a39edcdaf
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573217"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/external/connections/contosohr/schema"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"respond-async" forHTTPHeaderField:@"Prefer"];
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