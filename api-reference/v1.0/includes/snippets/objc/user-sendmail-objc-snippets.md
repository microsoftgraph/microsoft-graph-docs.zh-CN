---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 53b4dea93538d084df7c0c9fb5180cf470e7958b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711400"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/sendMail"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"Meet for lunch?"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType text]];
[body setContent:@"The new cafeteria is open."];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"fannyd@contoso.onmicrosoft.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];
NSMutableArray *ccRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *ccRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"danas@contoso.onmicrosoft.com"];
[ccRecipients setEmailAddress:emailAddress];
[ccRecipientsList addObject: ccRecipients];
[message setCcRecipients:ccRecipientsList];
payloadDictionary[@"message"] = message;

BOOL saveToSentItems = NO;
payloadDictionary[@"saveToSentItems"] = saveToSentItems;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```