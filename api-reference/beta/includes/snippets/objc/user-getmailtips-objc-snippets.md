---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e12741b3620cf6f1af14c6ffad66be34e673a9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608725"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/getMailTips"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *emailAddressesList = [[NSMutableArray alloc] init];
[emailAddressesList addObject: @"danas@contoso.onmicrosoft.com"];
[emailAddressesList addObject: @"fannyd@contoso.onmicrosoft.com"];
payloadDictionary[@"EmailAddresses"] = emailAddressesList;

MSGraphMailTipsType *mailTipsOptions = [MSGraphMailTipsType automaticReplies];
payloadDictionary[@"MailTipsOptions"] = mailTipsOptions;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```