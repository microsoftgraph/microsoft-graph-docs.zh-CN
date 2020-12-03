---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5970987227dec8e5d736f86a68533bf9b9b4bb8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524137"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/policies/permissionGrantPolicies/{id}/includes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPermissionGrantConditionSet *permissionGrantConditionSet = [[MSGraphPermissionGrantConditionSet alloc] init];
[permissionGrantConditionSet setPermissionType: [MSGraphPermissionType delegated]];
[permissionGrantConditionSet setClientApplicationsFromVerifiedPublisherOnly: true];

NSError *error;
NSData *permissionGrantConditionSetData = [permissionGrantConditionSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:permissionGrantConditionSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```