---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bd738b47efd69e02a9897f32970e949f4cfba0a8f9daa901886f038098e7a9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378830"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailboxSettings/automaticRepliesSetting"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAutomaticRepliesSetting *automaticRepliesSetting = [[MSGraphAutomaticRepliesSetting alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```