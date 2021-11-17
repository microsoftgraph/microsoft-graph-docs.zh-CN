---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7dfcf8cba95450dbb1ae1b67614bd7f27cb52aa8ab814551278cd170c016ecc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220179"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/webAccounts/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWebAccount *webAccount = [[MSGraphWebAccount alloc] init];
[webAccount setWebUrl:@"https://github.com/innocenty.popov"];

NSError *error;
NSData *webAccountData = [webAccount getSerializedDataWithError:&error];
[urlRequest setHTTPBody:webAccountData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```