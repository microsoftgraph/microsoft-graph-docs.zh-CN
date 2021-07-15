---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f7416b4bc10648e1adc41149bf1410a2647d416
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441996"
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