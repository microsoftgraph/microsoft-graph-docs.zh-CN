---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da5fa164559e6f8933782494280ab32454c51550
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960018"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeamsTab *teamsTab = [[MSGraphTeamsTab alloc] init];
[teamsTab setDisplayName:@"My Contoso Tab"];
MSGraphTeamsTabConfiguration *configuration = [[MSGraphTeamsTabConfiguration alloc] init];
[configuration setEntityId:@"2DCA2E6C7A10415CAF6B8AB6661B3154"];
[configuration setContentUrl:@"https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView"];
[configuration setWebsiteUrl:@"https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154"];
[configuration setRemoveUrl:@"https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"];
[teamsTab setConfiguration:configuration];

NSError *error;
NSData *teamsTabData = [teamsTab getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamsTabData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```