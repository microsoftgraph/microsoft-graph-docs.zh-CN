---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a32914f8040bd859cb0f9cf9f82c46e8e48550de
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35330726"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/tiIndicators/updateTiIndicators"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *valueList = [[NSMutableArray alloc] init];
MSGraphTiIndicator *value = [[MSGraphTiIndicator alloc] init];
[value setId:@"c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4"];
[value setAdditionalInformation:@"mytest"];
[valueList addObject: value];
MSGraphTiIndicator *value = [[MSGraphTiIndicator alloc] init];
[value setId:@"e58c072b-c9bb-a5c4-34ce-eb69af44fb1e"];
[value setAdditionalInformation:@"test again"];
[valueList addObject: value];
payloadDictionary[@"value"] = valueList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```