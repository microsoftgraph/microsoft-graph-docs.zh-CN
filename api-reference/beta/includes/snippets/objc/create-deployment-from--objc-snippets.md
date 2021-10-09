---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ad30ccf33c5cdfded68783220c2f07b50a5697ab7ae146b09571e3b5b6ac110
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104466"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/deployments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWindowsUpdatesDeployment *deployment = [[MSGraphWindowsUpdatesDeployment alloc] init];
MSGraphWindowsUpdatesDeployableContent *content = [[MSGraphWindowsUpdatesDeployableContent alloc] init];
[content setVersion:@"20H2"];
[deployment setContent:content];
MSGraphWindowsUpdatesDeploymentSettings *settings = [[MSGraphWindowsUpdatesDeploymentSettings alloc] init];
MSGraphWindowsUpdatesRolloutSettings *rollout = [[MSGraphWindowsUpdatesRolloutSettings alloc] init];
[rollout setDevicesPerOffer: 100];
[settings setRollout:rollout];
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