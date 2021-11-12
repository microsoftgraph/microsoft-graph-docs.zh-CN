---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba3596255a97be178e0ecd282c4d6dc1c58a285e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687470"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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