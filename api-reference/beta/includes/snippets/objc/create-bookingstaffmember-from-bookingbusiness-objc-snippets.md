---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d2b807ede6f6e1fe5f0269886f74bf3210b9eb8a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709626"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/{id}/staffMembers"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingStaffMember *bookingStaffMember = [[MSGraphBookingStaffMember alloc] init];
[bookingStaffMember setColorIndex: 1];
[bookingStaffMember setDisplayName:@"Dana Swope"];
[bookingStaffMember setEmailAddress:@"danas@contoso.com"];
[bookingStaffMember setRole: [MSGraphBookingStaffRole externalGuest]];
[bookingStaffMember setUseBusinessHours: true];
NSMutableArray *workingHoursList = [[NSMutableArray alloc] init];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek monday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
MSGraphBookingWorkTimeSlot *timeSlots = [[MSGraphBookingWorkTimeSlot alloc] init];
[timeSlots setEnd:@"17:00:00.0000000"];
[timeSlots setStart:@"08:00:00.0000000"];
[timeSlotsList addObject: timeSlots];
[workingHours setTimeSlots:timeSlotsList];
[workingHoursList addObject: workingHours];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek tuesday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
MSGraphBookingWorkTimeSlot *timeSlots = [[MSGraphBookingWorkTimeSlot alloc] init];
[timeSlots setEnd:@"17:00:00.0000000"];
[timeSlots setStart:@"08:00:00.0000000"];
[timeSlotsList addObject: timeSlots];
[workingHours setTimeSlots:timeSlotsList];
[workingHoursList addObject: workingHours];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek wednesday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
MSGraphBookingWorkTimeSlot *timeSlots = [[MSGraphBookingWorkTimeSlot alloc] init];
[timeSlots setEnd:@"17:00:00.0000000"];
[timeSlots setStart:@"08:00:00.0000000"];
[timeSlotsList addObject: timeSlots];
[workingHours setTimeSlots:timeSlotsList];
[workingHoursList addObject: workingHours];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek thursday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
MSGraphBookingWorkTimeSlot *timeSlots = [[MSGraphBookingWorkTimeSlot alloc] init];
[timeSlots setEnd:@"17:00:00.0000000"];
[timeSlots setStart:@"08:00:00.0000000"];
[timeSlotsList addObject: timeSlots];
[workingHours setTimeSlots:timeSlotsList];
[workingHoursList addObject: workingHours];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek friday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
MSGraphBookingWorkTimeSlot *timeSlots = [[MSGraphBookingWorkTimeSlot alloc] init];
[timeSlots setEnd:@"17:00:00.0000000"];
[timeSlots setStart:@"08:00:00.0000000"];
[timeSlotsList addObject: timeSlots];
[workingHours setTimeSlots:timeSlotsList];
[workingHoursList addObject: workingHours];
[bookingStaffMember setWorkingHours:workingHoursList];

NSError *error;
NSData *bookingStaffMemberData = [bookingStaffMember getSerializedDataWithError:&error];
[urlRequest setHTTPBody:bookingStaffMemberData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```