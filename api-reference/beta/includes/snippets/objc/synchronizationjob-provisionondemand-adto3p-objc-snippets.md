---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3aeb981a7544dbc4ed1ddeaf63e3c8ed1868987c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202901"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/c8c95753-f628-48e1-9fab-76c2d4cf624c/synchronization/jobs/3f7565a3-fde6-4e4d-bda8-1bb70aba3612/provisionOnDemand"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *parametersList = [[NSMutableArray alloc] init];
MSGraphSynchronizationJobApplicationParameters *parameters = [[MSGraphSynchronizationJobApplicationParameters alloc] init];
NSMutableArray *subjectsList = [[NSMutableArray alloc] init];
MSGraphSynchronizationJobSubject *subjects = [[MSGraphSynchronizationJobSubject alloc] init];
[subjects setObjectId:@"9bb0f679-a883-4a6f-8260-35b491b8b8c8"];
[subjects setObjectTypeName:@"User"];
[subjectsList addObject: subjects];
[parameters setSubjects:subjectsList];
[parameters setRuleId:@"ea807875-5618-4f0a-9125-0b46a05298ca"];
[parametersList addObject: parameters];
payloadDictionary[@"parameters"] = parametersList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```