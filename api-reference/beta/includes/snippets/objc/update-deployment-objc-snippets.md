---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5d3eeada22fe00f7d99b1074cc1e666c2bec6c7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241308"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/deployments/b5171742-1742-b517-4217-17b5421717b5"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWindowsUpdatesDeployment *deployment = [[MSGraphWindowsUpdatesDeployment alloc] init];
MSGraphWindowsUpdatesDeploymentSettings *settings = [[MSGraphWindowsUpdatesDeploymentSettings alloc] init];
MSGraphWindowsUpdatesMonitoringSettings *monitoring = [[MSGraphWindowsUpdatesMonitoringSettings alloc] init];
NSMutableArray *monitoringRulesList = [[NSMutableArray alloc] init];
MSGraphWindowsUpdatesMonitoringRule *monitoringRules = [[MSGraphWindowsUpdatesMonitoringRule alloc] init];
[monitoringRules setSignal: [MSGraphWindowsUpdatesMonitoringSignal rollback]];
[monitoringRules setThreshold: 5];
[monitoringRules setAction: [MSGraphWindowsUpdatesMonitoringAction pauseDeployment]];
[monitoringRulesList addObject: monitoringRules];
[monitoring setMonitoringRules:monitoringRulesList];
[settings setMonitoring:monitoring];
[deployment setSettings:settings];

NSError *error;
NSData *deploymentData = [deployment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:deploymentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```