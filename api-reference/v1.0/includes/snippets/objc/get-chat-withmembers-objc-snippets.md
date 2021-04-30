---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 832f3ff6c9c6f855c9b22d967108e1d7cfa5fc90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080594"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:b8577894a63548969c5c92bb9c80c5e1@thread.v2?$expand=members"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphChat *chat = [[MSGraphChat alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```