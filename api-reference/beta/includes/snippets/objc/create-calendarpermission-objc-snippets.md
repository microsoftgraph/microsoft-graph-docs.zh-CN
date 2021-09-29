---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 993346e8e4566b9b08f11684be6dc8482ff3c67e
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995684"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/458d4c95-124e-49da-ba9d-1dd0387e682e/calendar/calendarPermissions"]]];
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