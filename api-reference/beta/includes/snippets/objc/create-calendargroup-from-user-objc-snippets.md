---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e028c1da28bfce3d8dc98ab0daf18321dded4e99
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613019"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendarGroups"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCalendarGroup *calendarGroup = [[MSGraphCalendarGroup alloc] init];
[calendarGroup setName:@"name-value"];
[calendarGroup setClassId:@"classId-value"];
[calendarGroup setChangeKey:@"changeKey-value"];

NSError *error;
NSData *calendarGroupData = [calendarGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:calendarGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```