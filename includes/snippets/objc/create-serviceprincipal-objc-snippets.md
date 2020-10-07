---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b94eb1be790e87b29aebf18977625e17cdea586
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "48373293"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/serviceprincipals"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"appplication/json" forHTTPHeaderField:@"Content-Type"];

MSGraphServicePrincipal *servicePrincipal = [[MSGraphServicePrincipal alloc] init];
[servicePrincipal setAppId:@"d7fbfe28-c60e-46d2-8335-841923950d3b"];
NSMutableArray *tagsList = [[NSMutableArray alloc] init];
[tagsList addObject: @"WindowsAzureActiveDirectoryIntegratedApp"];
[tagsList addObject: @"WindowsAzureActiveDirectoryOnPremApp"];
[servicePrincipal setTags:tagsList];

NSError *error;
NSData *servicePrincipalData = [servicePrincipal getSerializedDataWithError:&error];
[urlRequest setHTTPBody:servicePrincipalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```