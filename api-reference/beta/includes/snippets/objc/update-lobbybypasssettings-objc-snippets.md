---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2799492871a9aaf176482ad25d5a953b0c7b6dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775596"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnlineMeeting *onlineMeeting = [[MSGraphOnlineMeeting alloc] init];
MSGraphLobbyBypassSettings *lobbyBypassSettings = [[MSGraphLobbyBypassSettings alloc] init];
[lobbyBypassSettings setIsDialInBypassEnabled: true];
[onlineMeeting setLobbyBypassSettings:lobbyBypassSettings];

NSError *error;
NSData *onlineMeetingData = [onlineMeeting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onlineMeetingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```