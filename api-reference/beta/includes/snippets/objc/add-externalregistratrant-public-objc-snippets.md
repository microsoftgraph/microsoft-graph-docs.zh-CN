---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 987ad932ceca49cb9e971e067660a0edf205e67b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118895"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrantBase *meetingRegistrantBase = [[MSGraphMeetingRegistrantBase alloc] init];
[meetingRegistrantBase setId:@"9d96988d-a66a-46ce-aad7-0b245615b297"];

NSError *error;
NSData *meetingRegistrantBaseData = [meetingRegistrantBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrantBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```