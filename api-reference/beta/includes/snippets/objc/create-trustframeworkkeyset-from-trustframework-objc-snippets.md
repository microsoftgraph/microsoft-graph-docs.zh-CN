---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e368fbc4de407a76b25546c3aad11f44fb68a91cb2d5cde11bf7c8f2dc90839
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279247"
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