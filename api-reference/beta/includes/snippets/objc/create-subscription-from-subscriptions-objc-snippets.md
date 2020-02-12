---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fd844c9a5f453b06696f1ea965da60d1c46390b
ms.sourcegitcommit: 1a84f80798692fc0381b1acecfe023b3ce6ab02c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2020
ms.locfileid: "41956443"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/subscriptions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSubscription *subscription = [[MSGraphSubscription alloc] init];
[subscription setChangeType:@"updated"];
[subscription setNotificationUrl:@"https://webhook.azurewebsites.net/api/send/myNotifyClient"];
[subscription setResource:@"me/mailFolders('Inbox')/messages"];
[subscription setExpirationDateTime: "2016-11-20T18:23:45.9356913Z"];
[subscription setClientState:@"secretClientValue"];
[subscription setLatestSupportedTlsVersion:@"v1_2"];

NSError *error;
NSData *subscriptionData = [subscription getSerializedDataWithError:&error];
[urlRequest setHTTPBody:subscriptionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```