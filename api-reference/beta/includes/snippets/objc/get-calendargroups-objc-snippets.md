---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ff2b3d0c8fa9c9852dd6341f3f5e0838f0139418
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500351"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendarGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *calendarGroupList = [[NSMutableArray alloc] init];
        calendarGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphCalendarGroup *calendarGroup = [[MSGraphCalendarGroup alloc] initWithDictionary:[calendarGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```