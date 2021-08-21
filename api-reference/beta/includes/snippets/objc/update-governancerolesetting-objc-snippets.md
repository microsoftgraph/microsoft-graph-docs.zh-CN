---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84e6225d5e1a1e7762720bc93c44cf68ac4f9ccf05d177b428d1c7889d43a7e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329042"
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