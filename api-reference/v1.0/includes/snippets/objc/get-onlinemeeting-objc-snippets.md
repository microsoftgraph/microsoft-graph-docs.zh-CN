---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 372212ab85ce1567594d09a7f76015b1f11a4c87
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865796"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *onlineMeetingList = [[NSMutableArray alloc] init];
        onlineMeetingList = [jsonFinal valueForKey:@"value"];
        MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] initWithDictionary:[onlineMeetingList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```