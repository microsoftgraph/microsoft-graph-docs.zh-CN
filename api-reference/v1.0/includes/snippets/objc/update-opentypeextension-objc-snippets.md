---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b44b703b8898a7eb2fa177d60af7814d17f354a7
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470713"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphExtension *extension = [[MSGraphExtension alloc] init];
[extension setExtensionName:@"Com.Contoso.Estimate"];
[extension setCompanyName:@"Contoso"];
[extension setExpirationDate: "2016-07-30T11:00:00Z"];
[extension setDealValue: 1010100];
NSMutableArray *topPicksList = [[NSMutableArray alloc] init];
[topPicksList addObject: @"Employees only"];
[topPicksList addObject: @"Add spouse or guest"];
[topPicksList addObject: @"Add family"];
[extension setTopPicks:topPicksList];

NSError *error;
NSData *extensionData = [extension getSerializedDataWithError:&error];
[urlRequest setHTTPBody:extensionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```