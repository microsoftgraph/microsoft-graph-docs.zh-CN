---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0624dcff041fec4face129c4097f42d130502d06
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938306"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/trustFramework/keySets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTrustFrameworkKeySet *trustFrameworkKeySet = [[MSGraphTrustFrameworkKeySet alloc] init];
[trustFrameworkKeySet setId:@"keyset1"];
NSMutableArray *keysList = [[NSMutableArray alloc] init];
MSGraphTrustFrameworkKey *keys = [[MSGraphTrustFrameworkKey alloc] init];
[keys setK:@"k-value"];
NSMutableArray *x5cList = [[NSMutableArray alloc] init];
[x5cList addObject: @"x5c-value"];
[keys setX5c:x5cList];
[keys setX5t:@"x5t-value"];
[keys setKty:@"kty-value"];
[keys setUse:@"use-value"];
[keys setExp: 99];
[keys setNbf: 99];
[keys setKid:@"kid-value"];
[keys setE:@"e-value"];
[keys setN:@"n-value"];
[keys setD:@"d-value"];
[keys setP:@"p-value"];
[keys setQ:@"q-value"];
[keys setDp:@"dp-value"];
[keys setDq:@"dq-value"];
[keys setQi:@"qi-value"];
[keysList addObject: keys];
[trustFrameworkKeySet setKeys:keysList];

NSError *error;
NSData *trustFrameworkKeySetData = [trustFrameworkKeySet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:trustFrameworkKeySetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```