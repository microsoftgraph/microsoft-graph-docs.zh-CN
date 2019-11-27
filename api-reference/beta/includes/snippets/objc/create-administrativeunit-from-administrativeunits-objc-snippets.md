---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 919ee91e8e47ca0e807217ab3919c874f9467fc8
ms.sourcegitcommit: fc9edd17aebed91768e31416e1c1ee0b64d5ce06
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39621593"
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