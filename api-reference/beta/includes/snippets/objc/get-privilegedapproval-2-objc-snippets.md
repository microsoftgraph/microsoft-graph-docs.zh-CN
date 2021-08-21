---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebb85882c413bbd0df56f89f9d754d88720e9d03daa418daf557f0b1e6f77dfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163101"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedApproval"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphPrivilegedApproval *privilegedApproval = [[MSGraphPrivilegedApproval alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```