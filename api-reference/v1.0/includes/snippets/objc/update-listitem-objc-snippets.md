---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7508471098d87e5d4d0636b46397623e1c06b146
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509659"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/lists/{list-id}/items/{item-id}/fields"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFieldValueSet *fieldValueSet = [[MSGraphFieldValueSet alloc] init];
[fieldValueSet setColor:@"Fuchsia"];
[fieldValueSet setQuantity: 934];

NSError *error;
NSData *fieldValueSetData = [fieldValueSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:fieldValueSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```