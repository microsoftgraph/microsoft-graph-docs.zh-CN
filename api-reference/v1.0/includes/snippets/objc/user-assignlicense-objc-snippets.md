---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9221a3f29d6df43a249a51af800307f1ecd85d4b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35468084"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/assignLicense"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *addLicensesList = [[NSMutableArray alloc] init];
MSGraphAssignedLicense *addLicenses = [[MSGraphAssignedLicense alloc] init];
NSMutableArray *disabledPlansList = [[NSMutableArray alloc] init];
[disabledPlansList addObject: @"11b0131d-43c8-4bbb-b2c8-e80f9a50834a"];
[addLicenses setDisabledPlans:disabledPlansList];
[addLicenses setSkuId:@"guid"];
[addLicensesList addObject: addLicenses];
payloadDictionary[@"addLicenses"] = addLicensesList;

NSMutableArray *removeLicensesList = [[NSMutableArray alloc] init];
[removeLicensesList addObject: @"bea13e0c-3828-4daa-a392-28af7ff61a0f"];
payloadDictionary[@"removeLicenses"] = removeLicensesList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```