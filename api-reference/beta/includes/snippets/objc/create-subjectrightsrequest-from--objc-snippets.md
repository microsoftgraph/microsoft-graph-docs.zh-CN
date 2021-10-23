---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ff9cd07d66d6d266ba9912de1cb0832a83e1bf9
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561785"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privacy/subjectRightsRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSubjectRightsRequest *subjectRightsRequest = [[MSGraphSubjectRightsRequest alloc] init];
[subjectRightsRequest setType: [MSGraphSubjectRightsRequestType export]];
[subjectRightsRequest setDataSubjectType: [MSGraphDataSubjectType customer]];
NSMutableArray *regulationsList = [[NSMutableArray alloc] init];
[regulationsList addObject: @"String"];
[subjectRightsRequest setRegulations:regulationsList];
[subjectRightsRequest setDisplayName:@"String"];
[subjectRightsRequest setDescription:@"String"];
[subjectRightsRequest setInternalDueDateTime:@"String (timestamp)"];
MSGraphDataSubject *dataSubject = [[MSGraphDataSubject alloc] init];
[dataSubject setFirstName:@"String"];
[dataSubject setLastName:@"String"];
[dataSubject setEmail:@"String"];
[dataSubject setResidency:@"String"];
[dataSubject setPhoneNumber:@"String"];
[dataSubject setSSN:@"String"];
[subjectRightsRequest setDataSubject:dataSubject];

NSError *error;
NSData *subjectRightsRequestData = [subjectRightsRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:subjectRightsRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```