---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb7aa42cd39573305d296500b4d113ae839a07c6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863528"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/timeOffRequests"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTimeOffRequest *timeOffRequests = [[MSGraphTimeOffRequest alloc] init];
[timeOffRequests setStartDateTime:@"datetime-value"];
[timeOffRequests setEndDateTime:@"datetime-value"];
[timeOffRequests setTimeOffReasonId:@"timeOffReasonId-value"];

NSError *error;
NSData *timeOffRequestsData = [timeOffRequests getSerializedDataWithError:&error];
[urlRequest setHTTPBody:timeOffRequestsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```