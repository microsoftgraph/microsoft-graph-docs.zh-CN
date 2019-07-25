---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b243c03046275bfe9e31f825b3bf9203c5e8e005
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724406"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"return=representation" forHTTPHeaderField:@"Prefer"];
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