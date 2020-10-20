---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82891eb3f6d151b8b287827bd988f208c8c34f9e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620768"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMessageRule *messageRule = [[MSGraphMessageRule alloc] init];
[messageRule setDisplayName:@"Important from partner"];
MSGraphMessageRuleActions *actions = [[MSGraphMessageRuleActions alloc] init];
[actions setMarkImportance: [MSGraphImportance high]];
[messageRule setActions:actions];

NSError *error;
NSData *messageRuleData = [messageRule getSerializedDataWithError:&error];
[urlRequest setHTTPBody:messageRuleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```