---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ef9c24fd8386e1724b6b5918d21aa457eb8d8942476e88f8fbe4285521b9f3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333409"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/profile/phones"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphItemPhone *itemPhone = [[MSGraphItemPhone alloc] init];
[itemPhone setDisplayName:@"Car Phone"];
[itemPhone setNumber:@"+7 499 342 22 13"];

NSError *error;
NSData *itemPhoneData = [itemPhone getSerializedDataWithError:&error];
[urlRequest setHTTPBody:itemPhoneData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```