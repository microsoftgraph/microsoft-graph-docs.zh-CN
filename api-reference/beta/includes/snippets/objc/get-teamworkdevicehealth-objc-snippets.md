---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06c949a299a5ad936d5d5a0dbba6ea89ac8bea16
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349022"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/devices/d8214fe3-4fe3-d821-e34f-21d8e34f21d8/health"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTeamworkDeviceHealth *teamworkDeviceHealth = [[MSGraphTeamworkDeviceHealth alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```