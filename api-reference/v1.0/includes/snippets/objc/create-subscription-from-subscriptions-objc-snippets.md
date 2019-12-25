---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5bd876eaf685d70386b4ad1f83651d5a1370347
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864122"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSubscription *subscription = [[MSGraphSubscription alloc] init];
[subscription setChangeType:@"updated"];
[subscription setNotificationUrl:@"https://webhook.azurewebsites.net/api/send/myNotifyClient"];
[subscription setResource:@"me/mailFolders('Inbox')/messages"];
[subscription setExpirationDateTime: "2016-11-20T18:23:45.9356913Z"];
[subscription setClientState:@"secretClientValue"];

NSError *error;
NSData *subscriptionData = [subscription getSerializedDataWithError:&error];
[urlRequest setHTTPBody:subscriptionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```