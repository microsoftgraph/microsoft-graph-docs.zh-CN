---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0044e6d989561cd01ba17a8f8958369d1ebe55a7
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368850"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMobilityManagementPolicy *mobilityManagementPolicy = [[MSGraphMobilityManagementPolicy alloc] init];
[mobilityManagementPolicy setComplianceUrl:@"https://portal.mg.contoso.com/?portalAction=Compliance"];
[mobilityManagementPolicy setDiscoveryUrl:@"https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc"];
[mobilityManagementPolicy setTermsOfUseUrl:@"https://portal.mg.contoso.com/TermsofUse.aspx"];

NSError *error;
NSData *mobilityManagementPolicyData = [mobilityManagementPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mobilityManagementPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```