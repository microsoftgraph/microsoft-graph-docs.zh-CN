---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce44fb0a56cbe2fe4eb4c5e537871cc851343df05516ea39525cefd7910d57aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106138"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphDeviceCompliancePolicySettingStateSummary *deviceCompliancePolicySettingStateSummary = [[MSGraphDeviceCompliancePolicySettingStateSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```