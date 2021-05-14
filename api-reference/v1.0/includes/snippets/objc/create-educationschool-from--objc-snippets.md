---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc93a5686b15a87f1e62c912f486b4b1ae556a3
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474815"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/schools"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationSchool *educationSchool = [[MSGraphEducationSchool alloc] init];
[educationSchool setDisplayName:@"String"];
[educationSchool setDescription:@"String"];
[educationSchool setExternalSource: [MSGraphEducationExternalSource sis]];
[educationSchool setExternalSourceDetail:@"String"];
[educationSchool setPrincipalEmail:@"String"];
[educationSchool setPrincipalName:@"String"];
[educationSchool setExternalPrincipalId:@"String"];
[educationSchool setLowestGrade:@"String"];
[educationSchool setHighestGrade:@"String"];
[educationSchool setSchoolNumber:@"String"];
[educationSchool setExternalId:@"String"];
[educationSchool setPhone:@"String"];
[educationSchool setFax:@"String"];
MSGraphIdentitySet *createdBy = [[MSGraphIdentitySet alloc] init];
[educationSchool setCreatedBy:createdBy];
MSGraphPhysicalAddress *address = [[MSGraphPhysicalAddress alloc] init];
[educationSchool setAddress:address];

NSError *error;
NSData *educationSchoolData = [educationSchool getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationSchoolData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```