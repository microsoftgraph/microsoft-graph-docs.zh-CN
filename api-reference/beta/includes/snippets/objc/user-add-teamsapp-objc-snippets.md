---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16bb751c45fcf33da948ae1b771bcfaedae65aab
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570041"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{id}/teamwork/installedApps"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphUserScopeTeamsAppInstallation *userScopeTeamsAppInstallation = [[MSGraphUserScopeTeamsAppInstallation alloc] init];

NSError *error;
NSData *userScopeTeamsAppInstallationData = [userScopeTeamsAppInstallation getSerializedDataWithError:&error];
[urlRequest setHTTPBody:userScopeTeamsAppInstallationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```