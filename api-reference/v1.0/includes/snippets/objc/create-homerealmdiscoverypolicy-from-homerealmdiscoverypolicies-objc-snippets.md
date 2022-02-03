---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c83c9f81a66a7870f8bf07558a380ec36d0b5802
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350859"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/homeRealmDiscoveryPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphHomeRealmDiscoveryPolicy *homeRealmDiscoveryPolicy = [[MSGraphHomeRealmDiscoveryPolicy alloc] init];
NSMutableArray *definitionList = [[NSMutableArray alloc] init];
[definitionList addObject: @"{"HomeRealmDiscoveryPolicy":
     {"AccelerateToFederatedDomain":true,
      "PreferredDomain":"federated.example.edu",
      "AlternateIdLogin":{"Enabled":true}}}"];
[homeRealmDiscoveryPolicy setDefinition:definitionList];
[homeRealmDiscoveryPolicy setDisplayName:@"displayName-value"];
[homeRealmDiscoveryPolicy setIsOrganizationDefault: true];

NSError *error;
NSData *homeRealmDiscoveryPolicyData = [homeRealmDiscoveryPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:homeRealmDiscoveryPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```