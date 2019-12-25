---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af65c388f2054e2d8faff880286c04ad86658587
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870787"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/swapShiftsChangeRequests"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSwapShiftsChangeRequest *swapShiftsChangeRequests = [[MSGraphSwapShiftsChangeRequest alloc] init];
[swapShiftsChangeRequests setRecipientShiftId:@"recipientShiftId-value"];

NSError *error;
NSData *swapShiftsChangeRequestsData = [swapShiftsChangeRequests getSerializedDataWithError:&error];
[urlRequest setHTTPBody:swapShiftsChangeRequestsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```