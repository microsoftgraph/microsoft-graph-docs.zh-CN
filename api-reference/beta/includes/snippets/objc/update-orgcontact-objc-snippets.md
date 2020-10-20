---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd7f5798d98521017bee7b162a725f2580c34bca
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611429"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/contacts/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOrgContact *orgContact = [[MSGraphOrgContact alloc] init];
NSMutableArray *businessPhonesList = [[NSMutableArray alloc] init];
[businessPhonesList addObject: @"businessPhones-value"];
[orgContact setBusinessPhones:businessPhonesList];
[orgContact setCity:@"city-value"];
[orgContact setCompanyName:@"companyName-value"];
[orgContact setCountry:@"country-value"];
[orgContact setDepartment:@"department-value"];
[orgContact setDisplayName:@"displayName-value"];

NSError *error;
NSData *orgContactData = [orgContact getSerializedDataWithError:&error];
[urlRequest setHTTPBody:orgContactData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```