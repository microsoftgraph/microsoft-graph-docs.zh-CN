---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3c0a512d98dbf873a95e3fda79e8918edc8f2922
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402349"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5"]]];
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