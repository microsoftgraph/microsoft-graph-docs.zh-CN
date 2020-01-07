---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 937f8ed45750ff42f21b19cc2165515e679aa31b
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951895"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/openShifts"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOpenShift *openShifts = [[MSGraphOpenShift alloc] init];
MSGraphOpenShiftItem *sharedOpenShift = [[MSGraphOpenShiftItem alloc] init];
[sharedOpenShift setOpenSlotCount: 99];
[openShifts setSharedOpenShift:sharedOpenShift];
MSGraphOpenShiftItem *draftOpenShift = [[MSGraphOpenShiftItem alloc] init];
[draftOpenShift setOpenSlotCount: 99];
[openShifts setDraftOpenShift:draftOpenShift];
[openShifts setSchedulingGroupId:@"TAG_f914d037-00a3-4ba4-b712-ef178cbea263"];

NSError *error;
NSData *openShiftsData = [openShifts getSerializedDataWithError:&error];
[urlRequest setHTTPBody:openShiftsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```