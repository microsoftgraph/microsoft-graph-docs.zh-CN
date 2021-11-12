---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 701303cc75b2c1990bd2c92bbe08b8d5590b92ea83f6ddce4491bd6aec8ee5da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158456"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule"]]];
[urlRequest setHTTPMethod:@"PUT"];

MSGraphSchedule *schedule = [[MSGraphSchedule alloc] init];
[schedule setEnabled: true];
[schedule setTimeZone:@"America/Chicago"];
[schedule setProvisionStatus: [MSGraphOperationStatus Completed]];
[schedule setProvisionStatusCode: null];
[schedule setOpenShiftsEnabled: true];
[schedule setSwapShiftsRequestsEnabled: true];
[schedule setOfferShiftRequestsEnabled: true];
[schedule setTimeOffRequestsEnabled: true];
[schedule setTimeClockEnabled: true];
MSGraphTimeClockSettings *timeClockSettings = [[MSGraphTimeClockSettings alloc] init];
MSGraphGeoCoordinates *approvedLocation = [[MSGraphGeoCoordinates alloc] init];
[approvedLocation setAltitude: 1024.13];
[approvedLocation setLatitude: 26.13246];
[approvedLocation setLongitude: 24.34616];
[timeClockSettings setApprovedLocation:approvedLocation];
[schedule setTimeClockSettings:timeClockSettings];

NSError *error;
NSData *scheduleData = [schedule getSerializedDataWithError:&error];
[urlRequest setHTTPBody:scheduleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```