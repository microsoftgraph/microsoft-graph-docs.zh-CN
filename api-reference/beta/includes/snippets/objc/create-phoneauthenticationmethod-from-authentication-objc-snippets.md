---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff8ef55f0227d3caf468568eafd98e29530b8ea5
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805712"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/phoneMethods"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPhoneAuthenticationMethod *phoneAuthenticationMethod = [[MSGraphPhoneAuthenticationMethod alloc] init];
[phoneAuthenticationMethod setPhoneNumber:@"+1 2065555555"];
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