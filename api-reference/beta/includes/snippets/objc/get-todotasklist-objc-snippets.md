---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed03fcff7e1c9c8192df41baae84bc8c8f03cea9
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873204"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/todo/lists/AAMkADIyAAAAABrJAAA="]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphAAMkADIyAAAAABrJAAA= *aAMkADIyAAAAABrJAAA= = [[MSGraphAAMkADIyAAAAABrJAAA= alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```