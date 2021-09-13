---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31429600fe08ad1df3ee4b549dcf2fac7350f2608587ede20426804efb45d306
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163030"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/calendars/AAMkAGViNDU9zAAAAAGtlAAA=/events"]]];
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
[event setIsOnlineMeeting: true];
[event setOnlineMeetingProvider: [MSGraphOnlineMeetingProviderType teamsForBusiness]];

NSError *error;
NSData *eventData = [event getSerializedDataWithError:&error];
[urlRequest setHTTPBody:eventData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```