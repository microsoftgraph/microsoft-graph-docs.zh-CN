---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ddf1de0a64307e22fa5871497ee564dde7807b8b8c7db51caebdb7ffbaeb611
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162423"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSubscription *subscription = [[MSGraphSubscription alloc] init];
[subscription setExpirationDateTime: "2016-11-22T18:23:45.9356913Z"];

NSError *error;
NSData *subscriptionData = [subscription getSerializedDataWithError:&error];
[urlRequest setHTTPBody:subscriptionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```