---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba23a682b9c52c383baf1c78112ba10f6c4e8eb1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771272"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphShiftPreferences *shiftPreferences = [[MSGraphShiftPreferences alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```