---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f3c94ec4fed0c99df13b1cde836ffa61d4cc5c98
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463746"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/administrativeUnits/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAdministrativeUnit *administrativeUnit = [[MSGraphAdministrativeUnit alloc] init];
[administrativeUnit setDisplayName:@"displayName-value"];
[administrativeUnit setDescription:@"description-value"];
[administrativeUnit setVisibility:@"visibility-value"];

NSError *error;
NSData *administrativeUnitData = [administrativeUnit getSerializedDataWithError:&error];
[urlRequest setHTTPBody:administrativeUnitData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```