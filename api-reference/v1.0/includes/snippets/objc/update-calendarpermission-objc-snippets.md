---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71bd08c1e1fd2403f0f3222837df86c106f20826
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806541"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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