---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4664fe13d6be74abb631a7dffc5c76934dc377238af9785e8fc36ecf42bcbe7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220255"
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