---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 124e9d4b3115575c33425c9932cc68ec231566f5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202874"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/3e916d82-dd59-4944-824d-93092908fd8d/synchronization/jobs/264ea562-28cd-42b1-93e0-8de1f0560581/provisionOnDemand"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *parametersList = [[NSMutableArray alloc] init];
MSGraphSynchronizationJobApplicationParameters *parameters = [[MSGraphSynchronizationJobApplicationParameters alloc] init];
[parameters setRuleId:@"6c409270-f78a-4bc6-af23-7cf3ab6482fe"];
NSMutableArray *subjectsList = [[NSMutableArray alloc] init];
MSGraphSynchronizationJobSubject *subjects = [[MSGraphSynchronizationJobSubject alloc] init];
[subjects setObjectId:@"CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com"];
[subjects setObjectTypeName:@"user"];
[subjectsList addObject: subjects];
[parameters setSubjects:subjectsList];
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