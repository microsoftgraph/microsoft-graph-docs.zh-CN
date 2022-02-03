---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53b17c0d6993e008dceab6870b1a815d65c1eca2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348763"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/synchronization/secrets"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationSecretKeyStringValuePair *secrets = [[MSGraphSynchronizationSecretKeyStringValuePair alloc] init];
NSMutableArray *valueList = [[NSMutableArray alloc] init];
MSGraphString *value = [[MSGraphString alloc] init];
[value setKey:@"BaseAddress"];
[value setValue:@"user@domain.com"];
[valueList addObject: value];
MSGraphString *value = [[MSGraphString alloc] init];
[value setKey:@"SecretToken"];
[value setValue:@"password-value"];
[valueList addObject: value];
MSGraphString *value = [[MSGraphString alloc] init];
[value setKey:@"SyncNotificationSettings"];
[value setValue:@"{\"Enabled\":false,\"DeleteThresholdEnabled\":false}"];
[valueList addObject: value];
MSGraphString *value = [[MSGraphString alloc] init];
[value setKey:@"SyncAll"];
[value setValue:@"false"];
[valueList addObject: value];
[secrets setValue:valueList];

NSError *error;
NSData *secretsData = [secrets getSerializedDataWithError:&error];
[urlRequest setHTTPBody:secretsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```