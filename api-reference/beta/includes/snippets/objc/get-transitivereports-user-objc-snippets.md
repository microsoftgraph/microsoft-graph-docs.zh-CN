---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eedf4df07b6d52effa4e405cff6c4727e24fc6c3ab16d47bea87516982c11c9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277932"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/45b7d2e7-b882-4a80-ba97-10b7a63b8fa4/transitiveReports/$count"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphInt32 *int32 = [[MSGraphInt32 alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```