---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 026acd80081e5f67ced6e92760f554d849253aa6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118896"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration/registrants"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMeetingRegistrantBase *meetingRegistrantBase = [[MSGraphMeetingRegistrantBase alloc] init];
[meetingRegistrantBase setId:@"30494ab7-7338-4592-bfec-a4333be2a0a6"];
[meetingRegistrantBase setTenantId:@"909c6581-5130-43e9-88f3-fcb3582cde37"];
[meetingRegistrantBase setUserId:@"cc515404-b55c-466e-b896-992c918ecc01"];

NSError *error;
NSData *meetingRegistrantBaseData = [meetingRegistrantBase getSerializedDataWithError:&error];
[urlRequest setHTTPBody:meetingRegistrantBaseData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```