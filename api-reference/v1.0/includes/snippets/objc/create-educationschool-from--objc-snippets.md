---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acb4ebe667f06b151e279070735541d7c48b0a958810631876dbf910df14d68a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902278"
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