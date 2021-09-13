---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71643907f03d56e7931f1ad2b28493b498e0ca45fa139d701831fcca644519e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104920"
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