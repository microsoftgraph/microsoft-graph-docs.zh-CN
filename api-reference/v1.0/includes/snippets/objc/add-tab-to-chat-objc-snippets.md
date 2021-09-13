---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 72748e04e9b7d9992d599a4ae4b0f6b784edf0447abfd19ac56bc24c1bb78fbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274089"
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