---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c28e6503997fed42321b0e5217a291880541f353f84e47ede7c10c92c5ea875f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162510"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeamsTab *teamsTab = [[MSGraphTeamsTab alloc] init];
[teamsTab setDisplayName:@"My Contoso Tab - updated again"];

NSError *error;
NSData *teamsTabData = [teamsTab getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamsTabData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```