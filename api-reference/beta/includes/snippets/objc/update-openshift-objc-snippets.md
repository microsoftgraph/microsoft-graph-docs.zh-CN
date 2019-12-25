---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db5e9b95cbb9b87fd43ac4ecee6d4a5a1a72cc31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867786"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/openShifts"]]];
[urlRequest setHTTPMethod:@"PATCH"];
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