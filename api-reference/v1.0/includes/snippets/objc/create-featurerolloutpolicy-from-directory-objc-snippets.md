---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 352459d3f1706dc9a7c865b1faf45ea89836b524308dcc64dddf3fa889c35180
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332781"
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