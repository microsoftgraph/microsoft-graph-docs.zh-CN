---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5daaf051de8ce07117e809e0a96eca245e66943
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201580"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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