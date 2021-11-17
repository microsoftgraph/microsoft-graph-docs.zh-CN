---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f75332a1457e4d53b238b5e078d5b0eb69063979d967f0982627b6d8d9e4ad24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903397"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/schedule/openShifts/OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOpenShift *openShift = [[MSGraphOpenShift alloc] init];
[openShift setSchedulingGroupId:@"TAG_228940ed-ff84-4e25-b129-1b395cf78be0"];
MSGraphOpenShiftItem *sharedOpenShift = [[MSGraphOpenShiftItem alloc] init];
[sharedOpenShift setNotes:@"Inventory Management"];
[sharedOpenShift setOpenSlotCount: 5];
[sharedOpenShift setDisplayName:@"Field shift"];
[sharedOpenShift setStartDateTime: "2018-10-04T00:58:45.34Z"];
[sharedOpenShift setEndDateTime: "2018-10-04T09:50:45.332Z"];
[sharedOpenShift setTheme: [MSGraphScheduleEntityTheme white]];
NSMutableArray *activitiesList = [[NSMutableArray alloc] init];
MSGraphShiftActivity *activities = [[MSGraphShiftActivity alloc] init];
[activities setIsPaid: true];
[activities setStartDateTime: "2018-10-04T00:58:45.34Z"];
[activities setEndDateTime: "2018-10-04T01:58:45.34Z"];
[activities setCode:@""];
[activities setDisplayName:@"Lunch"];
[activitiesList addObject: activities];
[sharedOpenShift setActivities:activitiesList];
[openShift setSharedOpenShift:sharedOpenShift];
[openShift setDraftOpenShift: null];

NSError *error;
NSData *openShiftData = [openShift getSerializedDataWithError:&error];
[urlRequest setHTTPBody:openShiftData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```