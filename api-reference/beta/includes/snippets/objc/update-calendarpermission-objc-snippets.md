---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a796053068c7084183a0b1f3a22c3d86843cc99
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994837"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/calendar/calendarPermissions/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCalendarPermission *calendarPermission = [[MSGraphCalendarPermission alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setName:@"My Organization"];
[calendarPermission setEmailAddress:emailAddress];
[calendarPermission setIsRemovable: true];
[calendarPermission setIsInsideOrganization: true];
[calendarPermission setRole: [MSGraphCalendarRoleType write]];
NSMutableArray *allowedRolesList = [[NSMutableArray alloc] init];
[allowedRolesList addObject: @"none"];
[allowedRolesList addObject: @"freeBusyRead"];
[allowedRolesList addObject: @"limitedRead"];
[allowedRolesList addObject: @"read"];
[allowedRolesList addObject: @"write"];
[calendarPermission setAllowedRoles:allowedRolesList];
[calendarPermission setId:@"RGVmYXVsdA=="];

NSError *error;
NSData *calendarPermissionData = [calendarPermission getSerializedDataWithError:&error];
[urlRequest setHTTPBody:calendarPermissionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```