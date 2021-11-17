---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d970f1b7dc0b293035c12d07478f6c633284bcb336b06f86bd436eec8d518ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220185"
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