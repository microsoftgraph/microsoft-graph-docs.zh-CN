---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3d403c6dcdf4ccb308f511576344eaf322e457884ed66bd33948f52f0ac1e7f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332602"
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