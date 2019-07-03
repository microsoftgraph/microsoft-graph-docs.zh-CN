---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9829527e72bafa62c52950def15fe70be71205e9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493177"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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