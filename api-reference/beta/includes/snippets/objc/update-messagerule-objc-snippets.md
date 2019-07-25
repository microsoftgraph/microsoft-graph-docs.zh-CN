---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82891eb3f6d151b8b287827bd988f208c8c34f9e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721381"
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