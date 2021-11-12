---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 222a8bb551dd0284cb685eea7f36eabc50f9b3f9e01d8896d1943191e240730d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161854"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers"]]];
[urlRequest setHTTPMethod:@"POST"];

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