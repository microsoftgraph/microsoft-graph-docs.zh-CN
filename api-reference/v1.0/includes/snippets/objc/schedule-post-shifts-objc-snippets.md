---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 582776fe68bd35fb7447359b5f2db733b19eb3740d0b6808f9654d23415fa285
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274209"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{teamId}/schedule/shifts"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphShift *shift = [[MSGraphShift alloc] init];
[shift setId:@"SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8"];
[shift setUserId:@"c5d0c76b-80c4-481c-be50-923cd8d680a1"];
[shift setSchedulingGroupId:@"TAG_228940ed-ff84-4e25-b129-1b395cf78be0"];
MSGraphShiftItem *sharedShift = [[MSGraphShiftItem alloc] init];
[sharedShift setDisplayName:@"Day shift"];
[sharedShift setNotes:@"Please do inventory as part of your shift."];
[sharedShift setStartDateTime: "2019-03-11T15:00:00Z"];
[sharedShift setEndDateTime: "2019-03-12T00:00:00Z"];
[sharedShift setTheme: [MSGraphScheduleEntityTheme blue]];
NSMutableArray *activitiesList = [[NSMutableArray alloc] init];
MSGraphShiftActivity *activities = [[MSGraphShiftActivity alloc] init];
[activities setIsPaid: true];
[activities setStartDateTime: "2019-03-11T15:00:00Z"];
[activities setEndDateTime: "2019-03-11T15:15:00Z"];
[activities setCode:@""];
[activities setDisplayName:@"Lunch"];
[activitiesList addObject: activities];
[sharedShift setActivities:activitiesList];
[shift setSharedShift:sharedShift];
MSGraphShiftItem *draftShift = [[MSGraphShiftItem alloc] init];
[draftShift setDisplayName:@"Day shift"];
[draftShift setNotes:@"Please do inventory as part of your shift."];
[draftShift setStartDateTime: "2019-03-11T15:00:00Z"];
[draftShift setEndDateTime: "2019-03-12T00:00:00Z"];
[draftShift setTheme: [MSGraphScheduleEntityTheme blue]];
NSMutableArray *activitiesList = [[NSMutableArray alloc] init];
MSGraphShiftActivity *activities = [[MSGraphShiftActivity alloc] init];
[activities setIsPaid: true];
[activities setStartDateTime: "2019-03-11T15:00:00Z"];
[activities setEndDateTime: "2019-03-11T15:30:00Z"];
[activities setCode:@""];
[activities setDisplayName:@"Lunch"];
[activitiesList addObject: activities];
[draftShift setActivities:activitiesList];
[shift setDraftShift:draftShift];

NSError *error;
NSData *shiftData = [shift getSerializedDataWithError:&error];
[urlRequest setHTTPBody:shiftData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```