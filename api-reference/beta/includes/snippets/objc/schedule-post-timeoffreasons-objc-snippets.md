---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d04ecfc79d7b5aa4d0899d1bb78447652d7b909
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613202"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timeOffReasons"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTimeOffReason *timeOffReason = [[MSGraphTimeOffReason alloc] init];
[timeOffReason setDisplayName:@"Vacation"];
[timeOffReason setIconType: [MSGraphTimeOffReasonIconType plane]];
[timeOffReason setIsActive: true];

NSError *error;
NSData *timeOffReasonData = [timeOffReason getSerializedDataWithError:&error];
[urlRequest setHTTPBody:timeOffReasonData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```