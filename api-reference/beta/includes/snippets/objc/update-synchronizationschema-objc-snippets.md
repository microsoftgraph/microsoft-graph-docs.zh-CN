---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22045121b45f8c1de0776dcd494fdad8a2a160e6eca0806c455d36cd55c9fd98
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164068"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationSchema *synchronizationSchema = [[MSGraphSynchronizationSchema alloc] init];
NSMutableArray *directoriesList = [[NSMutableArray alloc] init];
MSGraphDirectoryDefinition *directories = [[MSGraphDirectoryDefinition alloc] init];
[directories setName:@"Azure Active Directory"];
NSMutableArray *objectsList = [[NSMutableArray alloc] init];
MSGraphObjectDefinition *objects = [[MSGraphObjectDefinition alloc] init];
[objects setName:@"User"];
NSMutableArray *attributesList = [[NSMutableArray alloc] init];
MSGraphAttributeDefinition *attributes = [[MSGraphAttributeDefinition alloc] init];
[attributes setName:@"userPrincipalName"];
[attributes setType: [MSGraphAttributeType String]];
[attributesList addObject: attributes];
[objects setAttributes:attributesList];
[objectsList addObject: objects];
[directories setObjects:objectsList];
[directoriesList addObject: directories];
MSGraphDirectoryDefinition *directories = [[MSGraphDirectoryDefinition alloc] init];
[directories setName:@"Salesforce"];
[directoriesList addObject: directories];
[synchronizationSchema setDirectories:directoriesList];
NSMutableArray *synchronizationRulesList = [[NSMutableArray alloc] init];
MSGraphSynchronizationRule *synchronizationRules = [[MSGraphSynchronizationRule alloc] init];
[synchronizationRules setName:@"USER_TO_USER"];
[synchronizationRules setSourceDirectoryName:@"Azure Active Directory"];
[synchronizationRules setTargetDirectoryName:@"Salesforce"];
NSMutableArray *objectMappingsList = [[NSMutableArray alloc] init];
MSGraphObjectMapping *objectMappings = [[MSGraphObjectMapping alloc] init];
[objectMappings setSourceObjectName:@"User"];
[objectMappings setTargetObjectName:@"User"];
NSMutableArray *attributeMappingsList = [[NSMutableArray alloc] init];
MSGraphAttributeMapping *attributeMappings = [[MSGraphAttributeMapping alloc] init];
MSGraphAttributeMappingSource *source = [[MSGraphAttributeMappingSource alloc] init];
[attributeMappings setSource:source];
[attributeMappings setTargetAttributeName:@"userName"];
[attributeMappingsList addObject: attributeMappings];
[objectMappings setAttributeMappings:attributeMappingsList];
[objectMappingsList addObject: objectMappings];
[synchronizationRules setObjectMappings:objectMappingsList];
[synchronizationRulesList addObject: synchronizationRules];
[synchronizationSchema setSynchronizationRules:synchronizationRulesList];

NSError *error;
NSData *synchronizationSchemaData = [synchronizationSchema getSerializedDataWithError:&error];
[urlRequest setHTTPBody:synchronizationSchemaData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```