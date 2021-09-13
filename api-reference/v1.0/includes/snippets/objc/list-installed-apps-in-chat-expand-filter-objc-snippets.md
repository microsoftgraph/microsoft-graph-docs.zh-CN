---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9eb58717530abe21d266dddfcad9ddf9a9becd6a468dea12b0cb078c7d37ceea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106834"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps?$expand=teamsApp,teamsAppDefinition&$filter=teamsApp/externalId%20eq%20'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphTeamsAppInstallation *teamsAppInstallation = [[MSGraphTeamsAppInstallation alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```