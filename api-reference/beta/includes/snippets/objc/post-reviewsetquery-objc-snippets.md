---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8669cc0d15679e8f1359157ddd159bb44d1fff4e
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093670"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryReviewSetQuery *reviewSetQuery = [[MSGraphEdiscoveryReviewSetQuery alloc] init];
[reviewSetQuery setDisplayName:@"My Query 1"];
[reviewSetQuery setQuery:@"(subject:\"Quarterly Financials\")"];

NSError *error;
NSData *reviewSetQueryData = [reviewSetQuery getSerializedDataWithError:&error];
[urlRequest setHTTPBody:reviewSetQueryData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```