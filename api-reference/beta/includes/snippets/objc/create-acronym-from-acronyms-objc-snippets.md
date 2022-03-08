---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5994b5a296872617022276df0f5df19f23bb704
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338325"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/search/acronyms"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSearchAcronym *acronym = [[MSGraphSearchAcronym alloc] init];
[acronym setDisplayName:@"DNN"];
[acronym setStandsFor:@"Deep Neural Network"];
[acronym setDescription:@"A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."];
[acronym setWebUrl:@"http://microsoft.com/deep-neural-network"];
[acronym setState: [MSGraphSearchAnswerState draft]];

NSError *error;
NSData *acronymData = [acronym getSerializedDataWithError:&error];
[urlRequest setHTTPBody:acronymData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```