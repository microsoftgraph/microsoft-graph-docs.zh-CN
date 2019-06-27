---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c5a243c0108a772c27c225c8764e0637c23fc813
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330250"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGovernanceRoleSetting *governanceRoleSetting = [[MSGraphGovernanceRoleSetting alloc] init];
NSMutableArray *adminEligibleSettingsList = [[NSMutableArray alloc] init];
MSGraphGovernanceRuleSetting *adminEligibleSettings = [[MSGraphGovernanceRuleSetting alloc] init];
[adminEligibleSettings setRuleIdentifier:@"ExpirationRule"];
[adminEligibleSettings setSetting:@"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"];
[adminEligibleSettingsList addObject: adminEligibleSettings];
[governanceRoleSetting setAdminEligibleSettings:adminEligibleSettingsList];

NSError *error;
NSData *governanceRoleSettingData = [governanceRoleSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:governanceRoleSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```