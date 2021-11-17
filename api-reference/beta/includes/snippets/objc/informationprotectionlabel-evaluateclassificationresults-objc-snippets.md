---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7acd99e4a5181b3ed7869d78c9a6737277700329b61b8889d56bb69ff20b7684
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278299"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/policy/labels/evaluateClassificationResults"]]];
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