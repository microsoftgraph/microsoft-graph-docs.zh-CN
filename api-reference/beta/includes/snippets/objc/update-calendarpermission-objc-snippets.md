---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0ffb6d85c2da531a97e98d933e32b2a9b55227e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41778008"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/calendar/calendarPermissions/RGVmYXVsdA=="]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCalendarPermission *calendarPermission = [[MSGraphCalendarPermission alloc] init];
[calendarPermission setRole: [MSGraphCalendarRoleType write]];

NSError *error;
NSData *calendarPermissionData = [calendarPermission getSerializedDataWithError:&error];
[urlRequest setHTTPBody:calendarPermissionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```