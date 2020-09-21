---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc5e96df8c9f252d7d25a599c64e5329d6140dee
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565088"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/2eef613a-ca2d-42f4-89fe-84d5198ddedf/reviewSets/b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8/queries"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphReviewSetQuery *reviewSetQuery = [[MSGraphReviewSetQuery alloc] init];
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