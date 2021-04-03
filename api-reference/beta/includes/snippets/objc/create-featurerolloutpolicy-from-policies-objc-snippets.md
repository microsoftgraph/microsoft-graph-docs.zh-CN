---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3a23f5c2858a9a9603f6a4a971460e5bae8aa44
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508342"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/featureRolloutPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFeatureRolloutPolicy *featureRolloutPolicy = [[MSGraphFeatureRolloutPolicy alloc] init];
[featureRolloutPolicy setDisplayName:@"PassthroughAuthentication rollout policy"];
[featureRolloutPolicy setDescription:@"PassthroughAuthentication rollout policy"];
[featureRolloutPolicy setFeature: [MSGraphStagedFeatureName passthroughAuthentication]];
[featureRolloutPolicy setIsEnabled: true];
[featureRolloutPolicy setIsAppliedToOrganization: false];

NSError *error;
NSData *featureRolloutPolicyData = [featureRolloutPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:featureRolloutPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```