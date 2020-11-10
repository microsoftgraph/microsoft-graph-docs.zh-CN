---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01e10696b8288212c92a6c363aecbe7e81544504
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952919"
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