---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8476740025632732415a86cb7d535664d12c5473
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736643"
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
[bookingStaffMember setTimeZone:@"America/Chicago"];
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