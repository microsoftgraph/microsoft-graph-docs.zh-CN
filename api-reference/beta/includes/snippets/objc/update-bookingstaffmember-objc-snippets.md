---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30e64ce9a048469d7f084ca462e874d5f3b088d6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124089"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148"]]];
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