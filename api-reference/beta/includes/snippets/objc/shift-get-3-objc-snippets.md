---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dfbea1f486f51623cbb79e08157035623073b6c7577256857b8c3c468963b6c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903050"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/871dbd5c-3a6a-4392-bfe1-042452793a50/settings/shiftPreferences"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphShiftPreferences *shiftPreferences = [[MSGraphShiftPreferences alloc] init];
[shiftPreferences setId:@"SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7"];
NSMutableArray *availabilityList = [[NSMutableArray alloc] init];
MSGraphShiftAvailability *availability = [[MSGraphShiftAvailability alloc] init];
MSGraphPatternedRecurrence *recurrence = [[MSGraphPatternedRecurrence alloc] init];
MSGraphRecurrencePattern *pattern = [[MSGraphRecurrencePattern alloc] init];
[pattern setType: [MSGraphRecurrencePatternType weekly]];
NSMutableArray *daysOfWeekList = [[NSMutableArray alloc] init];
[daysOfWeekList addObject: @"Monday"];
[daysOfWeekList addObject: @"Wednesday"];
[daysOfWeekList addObject: @"Friday"];
[pattern setDaysOfWeek:daysOfWeekList];
[pattern setInterval: 1];
[recurrence setPattern:pattern];
MSGraphRecurrenceRange *range = [[MSGraphRecurrenceRange alloc] init];
[range setType: [MSGraphRecurrenceRangeType noEnd]];
[recurrence setRange:range];
[availability setRecurrence:recurrence];
[availability setTimeZone:@"Pacific Standard Time"];
[availability setTimeSlots: null];
[availabilityList addObject: availability];
[shiftPreferences setAvailability:availabilityList];

NSError *error;
NSData *shiftPreferencesData = [shiftPreferences getSerializedDataWithError:&error];
[urlRequest setHTTPBody:shiftPreferencesData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```