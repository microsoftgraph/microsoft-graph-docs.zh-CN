---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 283c7e0d7b1dfc18e5f47a8ab8a4049c172b14e18580b7f801b3e58063965893
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902559"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/administrativeUnits"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAdministrativeUnit *administrativeUnit = [[MSGraphAdministrativeUnit alloc] init];
[administrativeUnit setDisplayName:@"Seattle District Technical Schools"];
[administrativeUnit setDescription:@"Seattle district technical schools administration"];
[administrativeUnit setVisibility:@"HiddenMembership"];

NSError *error;
NSData *administrativeUnitData = [administrativeUnit getSerializedDataWithError:&error];
[urlRequest setHTTPBody:administrativeUnitData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```