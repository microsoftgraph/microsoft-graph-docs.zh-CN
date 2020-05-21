---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45b6fb3e4752fd2777980030695d66723e8f3fbb
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774802"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailboxSettings *mailboxSettings = [[MSGraphMailboxSettings alloc] init];
[mailboxSettings setDelegateMeetingMessageDeliveryOptions: [MSGraphDelegateMeetingMessageDeliveryOptions sendToDelegateAndPrincipal]];

NSError *error;
NSData *mailboxSettingsData = [mailboxSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailboxSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```