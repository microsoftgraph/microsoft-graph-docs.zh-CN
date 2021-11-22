---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 40bce5bab79db0a686b98b85a00e62696c5a76cc1fb5076b6e3750cfbaf6892a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332467"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWindowsUpdatesDeployment *deployment = [[MSGraphWindowsUpdatesDeployment alloc] init];
MSGraphWindowsUpdatesDeploymentState *state = [[MSGraphWindowsUpdatesDeploymentState alloc] init];
[state setRequestedValue: [MSGraphWindowsUpdatesRequestedDeploymentStateValue paused]];
[deployment setState:state];

NSError *error;
NSData *deploymentData = [deployment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:deploymentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```