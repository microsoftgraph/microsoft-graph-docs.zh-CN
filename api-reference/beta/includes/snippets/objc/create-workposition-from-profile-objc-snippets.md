---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c606324fa7b5a8ce01342294eb426fb2242c47c16a896351b741e6a9f34bea7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105533"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/positions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkPosition *workPosition = [[MSGraphWorkPosition alloc] init];
MSGraphPositionDetail *detail = [[MSGraphPositionDetail alloc] init];
MSGraphCompanyDetail *company = [[MSGraphCompanyDetail alloc] init];
[company setDisplayName:@"Adventureworks Ltd."];
[company setDepartment:@"Consulting"];
[company setOfficeLocation:@"AW23/344"];
MSGraphPhysicalAddress *address = [[MSGraphPhysicalAddress alloc] init];
[address setType: [MSGraphPhysicalAddressType business]];
[address setStreet:@"123 Patriachy Ponds"];
[address setCity:@"Moscow"];
[address setCountryOrRegion:@"Russian Federation"];
[address setPostalCode:@"RU-34621"];
[company setAddress:address];
[company setWebUrl:@"https://www.adventureworks.com"];
[detail setCompany:company];
[detail setJobTitle:@"Senior Product Branding Manager II"];
[detail setRole:@"consulting"];
[workPosition setDetail:detail];
[workPosition setIsCurrent: true];

NSError *error;
NSData *workPositionData = [workPosition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workPositionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```