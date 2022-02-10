---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 075b93ec13a08e7c4e0d686f0563b6e22575ed14
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519333"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directory/customSecurityAttributeDefinitions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCustomSecurityAttributeDefinition *customSecurityAttributeDefinition = [[MSGraphCustomSecurityAttributeDefinition alloc] init];
[customSecurityAttributeDefinition setAttributeSet:@"Engineering"];
[customSecurityAttributeDefinition setDescription:@"Active projects for user"];
[customSecurityAttributeDefinition setIsCollection: true];
[customSecurityAttributeDefinition setIsSearchable: true];
[customSecurityAttributeDefinition setName:@"Project"];
[customSecurityAttributeDefinition setStatus:@"Available"];
[customSecurityAttributeDefinition setType:@"String"];
[customSecurityAttributeDefinition setUsePreDefinedValuesOnly: true];
NSMutableArray *allowedValuesList = [[NSMutableArray alloc] init];
MSGraphAllowedValue *allowedValues = [[MSGraphAllowedValue alloc] init];
[allowedValues setId:@"Alpine"];
[allowedValues setIsActive: true];
[allowedValuesList addObject: allowedValues];
MSGraphAllowedValue *allowedValues = [[MSGraphAllowedValue alloc] init];
[allowedValues setId:@"Baker"];
[allowedValues setIsActive: true];
[allowedValuesList addObject: allowedValues];
MSGraphAllowedValue *allowedValues = [[MSGraphAllowedValue alloc] init];
[allowedValues setId:@"Cascade"];
[allowedValues setIsActive: true];
[allowedValuesList addObject: allowedValues];
[customSecurityAttributeDefinition setAllowedValues:allowedValuesList];

NSError *error;
NSData *customSecurityAttributeDefinitionData = [customSecurityAttributeDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:customSecurityAttributeDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```