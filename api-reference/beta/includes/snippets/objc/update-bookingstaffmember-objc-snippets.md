---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a12a3b418a1cbd06a1dfb9d990eac191caaa3065
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478819"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphBookingStaffMember *bookingStaffMember = [[MSGraphBookingStaffMember alloc] init];
NSMutableArray *workingHoursList = [[NSMutableArray alloc] init];
MSGraphBookingWorkHours *workingHours = [[MSGraphBookingWorkHours alloc] init];
[workingHours setDay: [MSGraphDayOfWeek monday]];
NSMutableArray *timeSlotsList = [[NSMutableArray alloc] init];
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