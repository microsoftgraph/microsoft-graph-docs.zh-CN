---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9801683a616df488f732321ac7e637e8f97e2a5d
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45008603"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/schemaExtensions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchemaExtension *schemaExtension = [[MSGraphSchemaExtension alloc] init];
[schemaExtension setId:@"courses"];
[schemaExtension setDescription:@"Graph Learn training courses extensions"];
NSMutableArray *targetTypesList = [[NSMutableArray alloc] init];
[targetTypesList addObject: @"Group"];
[schemaExtension setTargetTypes:targetTypesList];
[schemaExtension setOwner:@"50897f70-a455-4adf-87bc-4cf17091d5ac"];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"courseId"];
[properties setType:@"Integer"];
[propertiesList addObject: properties];
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"courseName"];
[properties setType:@"String"];
[propertiesList addObject: properties];
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"courseType"];
[properties setType:@"String"];
[propertiesList addObject: properties];
[schemaExtension setProperties:propertiesList];

NSError *error;
NSData *schemaExtensionData = [schemaExtension getSerializedDataWithError:&error];
[urlRequest setHTTPBody:schemaExtensionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```