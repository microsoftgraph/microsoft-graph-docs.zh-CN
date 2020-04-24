---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ead06229a4aecaa8b45859cf135a52b544df125
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805849"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPhoneAuthenticationMethod *phoneAuthenticationMethod = [[MSGraphPhoneAuthenticationMethod alloc] init];
[phoneAuthenticationMethod setPhoneNumber:@"+1 2065555554"];
[phoneAuthenticationMethod setPhoneType: [MSGraphAuthenticationPhoneType mobile]];

NSError *error;
NSData *phoneAuthenticationMethodData = [phoneAuthenticationMethod getSerializedDataWithError:&error];
[urlRequest setHTTPBody:phoneAuthenticationMethodData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```