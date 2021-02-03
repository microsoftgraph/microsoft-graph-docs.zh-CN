---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b79a729e5dac9bbbb76e56089ef9b80ce77a6a6b
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093722"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/compliance/ediscovery/cases/6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d/reviewSets"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEdiscoveryReviewSet *reviewSet = [[MSGraphEdiscoveryReviewSet alloc] init];
[reviewSet setDisplayName:@"My Reviewset 3"];

NSError *error;
NSData *reviewSetData = [reviewSet getSerializedDataWithError:&error];
[urlRequest setHTTPBody:reviewSetData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```