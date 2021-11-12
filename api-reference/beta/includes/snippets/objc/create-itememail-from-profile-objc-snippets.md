---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a86ebb44407ef7b962962fdca6fc39092f0d200287bb5443c1961114ee3a0ad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219529"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/emails"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemEmail *itemEmail = [[MSGraphItemEmail alloc] init];
[itemEmail setAddress:@"Innocenty.Popov@adventureworks.com"];

NSError *error;
NSData *itemEmailData = [itemEmail getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemEmailData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```