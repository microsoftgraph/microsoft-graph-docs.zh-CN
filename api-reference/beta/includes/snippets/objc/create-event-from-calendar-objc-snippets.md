---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b328bac14592e22362ca6e708e4131de7d268c9399286a242b30e31f3000f6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104022"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEvent *event = [[MSGraphEvent alloc] init];
[event setSubject:@"Let's go for lunch"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Does next month work for you?"];
[event setBody:body];
MSGraphDateTimeTimeZone *start = [[MSGraphDateTimeTimeZone alloc] init];
[start setDateTime: "2019-03-10T12:00:00"];
[start setTimeZone:@"Pacific Standard Time"];
[event setStart:start];
MSGraphDateTimeTimeZone *end = [[MSGraphDateTimeTimeZone alloc] init];
[end setDateTime: "2019-03-10T14:00:00"];
[end setTimeZone:@"Pacific Standard Time"];
[event setEnd:end];
MSGraphLocation *location = [[MSGraphLocation alloc] init];
[location setDisplayName:@"Harry's Bar"];
[event setLocation:location];
NSMutableArray *attendeesList = [[NSMutableArray alloc] init];
MSGraphAttendee *attendees = [[MSGraphAttendee alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"adelev@contoso.onmicrosoft.com"];
[emailAddress setName:@"Adele Vance"];
[attendees setEmailAddress:emailAddress];
[attendees setType: [MSGraphAttendeeType required]];
[attendeesList addObject: attendees];
[event setAttendees:attendeesList];
[event setTransactionId:@"7E163156-7762-4BEB-A1C6-729EA81755A7"];

NSError *error;
NSData *eventData = [event getSerializedDataWithError:&error];
[urlRequest setHTTPBody:eventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```