---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 343c2c0eb318e5aadab79cc2f3937ec322fae15159ecf3bc37888b83f3d955d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/tiIndicators/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTiIndicator *tiIndicator = [[MSGraphTiIndicator alloc] init];
[tiIndicator setDescription:@"description-updated"];

NSError *error;
NSData *tiIndicatorData = [tiIndicator getSerializedDataWithError:&error];
[urlRequest setHTTPBody:tiIndicatorData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```