---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50592153e6e3f119ec384e7b4fee7050a0c8890b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771853"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/{printerId}/taskTriggers"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrintTaskTrigger *printTaskTrigger = [[MSGraphPrintTaskTrigger alloc] init];
[printTaskTrigger setEvent: [MSGraphPrintEvent jobStarted]];

NSError *error;
NSData *printTaskTriggerData = [printTaskTrigger getSerializedDataWithError:&error];
[urlRequest setHTTPBody:printTaskTriggerData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```