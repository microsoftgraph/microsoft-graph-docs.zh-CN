---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 632f0ff029860aad453ec8af4736dc37c32096ee
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338334"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/search/acronyms/{acronymsId}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSearchAcronym *acronym = [[MSGraphSearchAcronym alloc] init];
[acronym setDescription:@"A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."];

NSError *error;
NSData *acronymData = [acronym getSerializedDataWithError:&error];
[urlRequest setHTTPBody:acronymData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```