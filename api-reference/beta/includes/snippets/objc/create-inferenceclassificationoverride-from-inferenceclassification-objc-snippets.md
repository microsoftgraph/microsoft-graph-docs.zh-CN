---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d9c0e9d704035b0accca3f1af433d996372f70b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705235"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/inferenceClassification/overrides"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphInferenceClassificationOverride *inferenceClassificationOverride = [[MSGraphInferenceClassificationOverride alloc] init];
[inferenceClassificationOverride setClassifyAs: [MSGraphInferenceClassificationType focused]];
MSGraphEmailAddress *senderEmailAddress = [[MSGraphEmailAddress alloc] init];
[senderEmailAddress setName:@"Samantha Booth"];
[senderEmailAddress setAddress:@"samanthab@adatum.onmicrosoft.com"];
[inferenceClassificationOverride setSenderEmailAddress:senderEmailAddress];

NSError *error;
NSData *inferenceClassificationOverrideData = [inferenceClassificationOverride getSerializedDataWithError:&error];
[urlRequest setHTTPBody:inferenceClassificationOverrideData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```