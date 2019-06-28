---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d5c0db008395fccabe8b37b4d583f65e53a26c34
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35322967"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/schools"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationSchool *educationSchool = [[MSGraphEducationSchool alloc] init];
[educationSchool setDisplayName:@"Fabrikam High School"];
[educationSchool setDescription:@"Magnate school for the arts. Los Angeles School District"];
[educationSchool setStatus:@"String"];
[educationSchool setExternalSource: [MSGraphEducationExternalSource sis]];
[educationSchool setPrincipalEmail:@"AmyR@fabrikam.com"];
[educationSchool setPrincipalName:@"Amy Roebuck"];
[educationSchool setExternalPrincipalId:@"14007"];
[educationSchool setHighestGrade:@"12"];
[educationSchool setLowestGrade:@"9"];
[educationSchool setSchoolNumber:@"10002"];
MSGraphPhysicalAddress *address = [[MSGraphPhysicalAddress alloc] init];
[address setCity:@"Los Angeles"];
[address setCountryOrRegion:@"United States"];
[address setPostalCode:@"98055"];
[address setState:@"CA"];
[address setStreet:@"12345 Main St."];
[educationSchool setAddress:address];
[educationSchool setExternalId:@"10002"];
[educationSchool setFax:@"+1 (253) 555-0101"];
[educationSchool setPhone:@"+1 (253) 555-0102"];

NSError *error;
NSData *educationSchoolData = [educationSchool getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationSchoolData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```