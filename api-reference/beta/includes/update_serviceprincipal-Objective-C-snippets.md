---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bdf160ca450711cd00fc1bf1db98d32985ad924f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35329873"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphServicePrincipal *servicePrincipal = [[MSGraphServicePrincipal alloc] init];
[servicePrincipal setAccountEnabled: true];
NSMutableArray *addInsList = [[NSMutableArray alloc] init];
MSGraphAddIn *addIns = [[MSGraphAddIn alloc] init];
[addIns setId:@"id-value"];
[addIns setType:@"type-value"];
NSMutableArray *propertiesList = [[NSMutableArray alloc] init];
MSGraphKeyValue *properties = [[MSGraphKeyValue alloc] init];
[properties setKey:@"key-value"];
[properties setValue:@"value-value"];
[propertiesList addObject: properties];
[addIns setProperties:propertiesList];
[addInsList addObject: addIns];
[servicePrincipal setAddIns:addInsList];
[servicePrincipal setAppDisplayName:@"appDisplayName-value"];
[servicePrincipal setAppId:@"appId-value"];
[servicePrincipal setAppOwnerOrganizationId:@"appOwnerOrganizationId-value"];
[servicePrincipal setAppRoleAssignmentRequired: true];

NSError *error;
NSData *servicePrincipalData = [servicePrincipal getSerializedDataWithError:&error];
[urlRequest setHTTPBody:servicePrincipalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```