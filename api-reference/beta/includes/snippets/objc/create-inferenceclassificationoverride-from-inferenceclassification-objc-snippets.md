---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d9c0e9d704035b0accca3f1af433d996372f70b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620741"
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