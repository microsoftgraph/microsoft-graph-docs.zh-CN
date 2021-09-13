---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3da3ad1efbac4430e8e9c387e8212fc1edd55a139de7a8cb3b1607179fc64696
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163506"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events/{id}/decline"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *comment = @"I won't be able to make this week. How about next week?";
payloadDictionary[@"comment"] = comment;

BOOL sendResponse = YES;
payloadDictionary[@"sendResponse"] = sendResponse;

MSGraphTimeSlot *proposedNewTime = [[MSGraphTimeSlot alloc] init];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2019-12-02T18:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[proposedNewTime setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2019-12-02T19:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[proposedNewTime setEnd:end];
payloadDictionary[@"proposedNewTime"] = proposedNewTime;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```