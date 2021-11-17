---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 445622ac4c20d3eadaa1d848acbec9356b811f1ec40d30ae9487563988228f6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219827"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps"]]];
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