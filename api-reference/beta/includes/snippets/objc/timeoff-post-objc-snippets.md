---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b6b44e5139072fca44194022733420c763fdbd25e4ba26da803810f457f6ab8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219425"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timesOff"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTimeOff *timeOff = [[MSGraphTimeOff alloc] init];
[timeOff setUserId:@"c5d0c76b-80c4-481c-be50-923cd8d680a1"];
MSGraphTimeOffItem *sharedTimeOff = [[MSGraphTimeOffItem alloc] init];
[sharedTimeOff setTimeOffReasonId:@"TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"];
[sharedTimeOff setStartDateTime: "2019-03-11T07:00:00Z"];
[sharedTimeOff setEndDateTime: "2019-03-12T07:00:00Z"];
[sharedTimeOff setTheme: [MSGraphScheduleEntityTheme white]];
[timeOff setSharedTimeOff:sharedTimeOff];
MSGraphTimeOffItem *draftTimeOff = [[MSGraphTimeOffItem alloc] init];
[draftTimeOff setTimeOffReasonId:@"TOR_891045ca-b5d2-406b-aa06-a3c8921245d7"];
[draftTimeOff setStartDateTime: "2019-03-11T07:00:00Z"];
[draftTimeOff setEndDateTime: "2019-03-12T07:00:00Z"];
[draftTimeOff setTheme: [MSGraphScheduleEntityTheme pink]];
[timeOff setDraftTimeOff:draftTimeOff];

NSError *error;
NSData *timeOffData = [timeOff getSerializedDataWithError:&error];
[urlRequest setHTTPBody:timeOffData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```