---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7746e495ceec40a3ae818c399c2a92488e2e18e
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996211"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendar/calendarPermissions"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphCalendarPermission *calendarPermission = [[MSGraphCalendarPermission alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setName:@"Samantha Booth"];
[emailAddress setAddress:@"samanthab@adatum.onmicrosoft.com"];
[calendarPermission setEmailAddress:emailAddress];
[calendarPermission setIsInsideOrganization: true];
[calendarPermission setIsRemovable: true];
[calendarPermission setRole: [MSGraphCalendarRoleType read]];

NSError *error;
NSData *calendarPermissionData = [calendarPermission getSerializedDataWithError:&error];
[urlRequest setHTTPBody:calendarPermissionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```