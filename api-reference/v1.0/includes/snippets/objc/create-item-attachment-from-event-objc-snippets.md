---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a16c0a8df8961c8fb37aebf941f8ae40b42bc334
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473816"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/events/AAMkAGI1AAAt9AHjAAA=/attachments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAttachment *attachment = [[MSGraphAttachment alloc] init];
[attachment setName:@"Holiday event"];
MSGraphOutlookItem *item = [[MSGraphOutlookItem alloc] init];
[item setSubject:@"Discuss gifts for children"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Let's look for funding!"];
[item setBody:body];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2016-12-02T18:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[item setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2016-12-02T19:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[item setEnd:end];
[attachment setItem:item];

NSError *error;
NSData *attachmentData = [attachment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:attachmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```