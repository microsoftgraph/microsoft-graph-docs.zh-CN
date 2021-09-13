---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a81a40a04bb6bda7db2659d27f7ce365473d89c8c3dbfc8c65a790b2be93a6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218759"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA="]]];
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