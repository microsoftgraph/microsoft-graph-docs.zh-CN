---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d849d07c748c1c1bab8cd44e6784c80143635fa0
ms.sourcegitcommit: 6deec57c0ab736260ee3599703bfd3f567ee6d82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "35738338"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSubscription *subscription = [[MSGraphSubscription alloc] init];
[subscription setChangeType:@"created,updated"];
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