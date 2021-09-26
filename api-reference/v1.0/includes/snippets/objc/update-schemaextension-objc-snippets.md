---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f055fc926888ad6e86ab780887eaf84668e966c
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764675"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/schemaExtensions/exto6x7sfft_courses"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSchemaExtension *schemaExtension = [[MSGraphSchemaExtension alloc] init];
[schemaExtension setOwner:@"ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa"];
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
MSGraphExtensionSchemaProperty *properties = [[MSGraphExtensionSchemaProperty alloc] init];
[properties setName:@"courseSupervisors"];
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