---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75a1fb501fcaf76d60f692564689f547c68d8a85fe064d4f8e07f27b8acaf0cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163670"
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