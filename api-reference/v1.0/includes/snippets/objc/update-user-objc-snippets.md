---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35e39c20ae0ad23c9ccc70006e3ec1a1364bf5d8e2b85054085579344b7e2d05
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161336"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUser *user = [[MSGraphUser alloc] init];
NSMutableArray *businessPhonesList = [[NSMutableArray alloc] init];
[businessPhonesList addObject: @"+1 425 555 0109"];
[user setBusinessPhones:businessPhonesList];
[user setOfficeLocation:@"18/2111"];

NSError *error;
NSData *userData = [user getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```