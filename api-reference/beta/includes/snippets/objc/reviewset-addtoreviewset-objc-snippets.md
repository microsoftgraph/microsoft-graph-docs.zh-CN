---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91a08f740368f3f8570c1513e5e0479c71533fb26ddebe7b7b756f03788ddebb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218567"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphEdiscoverySourceCollection *sourceCollection = [[MSGraphEdiscoverySourceCollection alloc] init];
[sourceCollection setId:@"1a9b4145d8f84e39bc45a7f68c5c5119"];
payloadDictionary[@"sourceCollection"] = sourceCollection;

MSGraphEdiscoveryAdditionalDataOptions *additionalData = [MSGraphEdiscoveryAdditionalDataOptions linkedFiles];
payloadDictionary[@"additionalData"] = additionalData;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```