---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b4009e6253c054d75ad6b306a613858b5773ccc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347423"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/devices/1ae3fe60-fe60-1ae3-60fe-e31a60fee31a/activity"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTeamworkDeviceActivity *teamworkDeviceActivity = [[MSGraphTeamworkDeviceActivity alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```