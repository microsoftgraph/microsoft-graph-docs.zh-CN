---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5987ba5384254e6cda9e7a742d0dbeb3ea95db2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995620"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationprotection/policy/labels/evaluateClassificationResults"]]];
[urlRequest setHTTPMethod:@"POST"];
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