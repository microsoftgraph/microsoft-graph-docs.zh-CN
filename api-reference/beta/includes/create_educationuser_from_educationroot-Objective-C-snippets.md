---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a24d03dc4f83a07b760cb59e7ae90cb9a8a33059
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318374"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/users"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationUser *educationUser = [[MSGraphEducationUser alloc] init];
[educationUser setDisplayName:@"Dion Matheson"];
[educationUser setGivenName:@"Dion"];
[educationUser setMiddleName: null];
[educationUser setSurname:@"Matheson"];
[educationUser setMail:@"DionM@contoso.com"];
[educationUser setMobilePhone:@"+1 (253) 555-0101"];
MSGraphIdentitySet *createdBy = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setDisplayName:@"Susana Rocha"];
[user setId:@"14012"];
[createdBy setUser:user];
[educationUser setCreatedBy:createdBy];
[educationUser setExternalSource: [MSGraphEducationExternalSource sis]];
MSGraphPhysicalAddress *mailingAddress = [[MSGraphPhysicalAddress alloc] init];
[mailingAddress setCity:@"Los Angeles"];
[mailingAddress setCountryOrRegion:@"United States"];
[mailingAddress setPostalCode:@"98055"];
[mailingAddress setState:@"CA"];
[mailingAddress setStreet:@"12345 Main St."];
[educationUser setMailingAddress:mailingAddress];
[educationUser setPrimaryRole: [MSGraphEducationUserRole student]];
MSGraphPhysicalAddress *residenceAddress = [[MSGraphPhysicalAddress alloc] init];
[residenceAddress setCity:@"Los Angeles"];
[residenceAddress setCountryOrRegion:@"United States"];
[residenceAddress setPostalCode:@"98055"];
[residenceAddress setState:@"CA"];
[residenceAddress setStreet:@"12345 Main St."];
[educationUser setResidenceAddress:residenceAddress];

NSError *error;
NSData *educationUserData = [educationUser getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationUserData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```