---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d83191746838d72c9ec55938b1edb5865300f061
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343823"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teamwork/devices/e19229ed-29ed-e192-ed29-92e1ed2992e1/configuration"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphTeamworkDeviceConfiguration *teamworkDeviceConfiguration = [[MSGraphTeamworkDeviceConfiguration alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```