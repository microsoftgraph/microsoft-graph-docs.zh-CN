---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93785fc5014dc08bcc13d49798bf6024e3c67ccd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865863"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] init];
[onlineMeeting setStartDateTime: "2019-07-12T21:30:34.2444915+00:00"];
[onlineMeeting setEndDateTime: "2019-07-12T22:00:34.2464912+00:00"];
[onlineMeeting setSubject:@"User Token Meeting"];

NSError *error;
NSData *onlineMeetingData = [onlineMeeting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onlineMeetingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```