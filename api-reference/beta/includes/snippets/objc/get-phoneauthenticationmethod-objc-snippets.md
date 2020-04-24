---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36bcd5433584a55f4c1750f2a45112ac827903b5
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806408"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphPhoneAuthenticationMethod *phoneAuthenticationMethod = [[MSGraphPhoneAuthenticationMethod alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```