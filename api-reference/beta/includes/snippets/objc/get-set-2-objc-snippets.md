---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcaa1f720a602a2bc8e16d9cefef895c4cfcc3b043a0da6ad2c287529b0a683
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277980"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/8ed8c9ea-7052-4c1d-a4d7-b9c10bffea6f"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphSet *set = [[MSGraphSet alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```