---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 25358b9a11fc9e5b74086fe43229a28a2fb3aac4107ef815425adbde49d5d653
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240547"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events/AAMkADAGu0AABIGYDaAAA="]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphEvent *event = [[MSGraphEvent alloc] init];
[event setIsOnlineMeeting: true];
[event setOnlineMeetingProvider: [MSGraphOnlineMeetingProviderType teamsForBusiness]];

NSError *error;
NSData *eventData = [event getSerializedDataWithError:&error];
[urlRequest setHTTPBody:eventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```