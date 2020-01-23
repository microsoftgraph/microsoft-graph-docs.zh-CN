---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa081b21984216e9bc80b0e7da618ecc26b8c4a4
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41495059"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationprotection/policy/labels/evaluateClassificationResults"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"ContosoLOBApp/1.0" forHTTPHeaderField:@"User-Agent"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphContentInfo *contentInfo = [[MSGraphContentInfo alloc] init];
[contentInfo setFormat: [MSGraphContentFormat default]];
[contentInfo setIdentifier: null];
[contentInfo setState: [MSGraphContentState rest]];
payloadDictionary[@"contentInfo"] = contentInfo;

NSMutableArray *classificationResultsList = [[NSMutableArray alloc] init];
MSGraphClassificationResult *classificationResults = [[MSGraphClassificationResult alloc] init];
[classificationResults setSensitiveTypeId:@"cb353f78-2b72-4c3c-8827-92ebe4f69fdf"];
[classificationResults setCount: 4];
[classificationResults setConfidenceLevel: 75];
[classificationResultsList addObject: classificationResults];
payloadDictionary[@"classificationResults"] = classificationResultsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```