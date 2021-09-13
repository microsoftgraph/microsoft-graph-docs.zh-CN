---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e4c25a0363cba0cc8614d7ce3dfd50db9d92c6f6fe792aca9dc3bec726e0f72
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161977"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/sendMail"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
[message setSubject:@"9/9/2018: concert"];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"The group represents Nevada."];
[message setBody:body];
NSMutableArray *toRecipientsList = [[NSMutableArray alloc] init];
MSGraphRecipient *toRecipients = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setAddress:@"AlexW@contoso.OnMicrosoft.com"];
[toRecipients setEmailAddress:emailAddress];
[toRecipientsList addObject: toRecipients];
[message setToRecipients:toRecipientsList];
NSMutableArray *internetMessageHeadersList = [[NSMutableArray alloc] init];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-name"];
[internetMessageHeaders setValue:@"Nevada"];
[internetMessageHeadersList addObject: internetMessageHeaders];
MSGraphInternetMessageHeader *internetMessageHeaders = [[MSGraphInternetMessageHeader alloc] init];
[internetMessageHeaders setName:@"x-custom-header-group-id"];
[internetMessageHeaders setValue:@"NV001"];
[internetMessageHeadersList addObject: internetMessageHeaders];
[message setInternetMessageHeaders:internetMessageHeadersList];
payloadDictionary[@"message"] = message;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```