---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de618a799c45d9ed381ab82da23a958dcfc657e1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440346"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMobilityManagementPolicy *mobilityManagementPolicy = [[MSGraphMobilityManagementPolicy alloc] init];
[mobilityManagementPolicy setComplianceUrl:@"https://portal.uem.contoso.com/?portalAction=Compliance"];
[mobilityManagementPolicy setDiscoveryUrl:@"https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc"];
[mobilityManagementPolicy setTermsOfUseUrl:@"https://portal.uem.contoso.com/TermsofUse.aspx"];

NSError *error;
NSData *mobilityManagementPolicyData = [mobilityManagementPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mobilityManagementPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```