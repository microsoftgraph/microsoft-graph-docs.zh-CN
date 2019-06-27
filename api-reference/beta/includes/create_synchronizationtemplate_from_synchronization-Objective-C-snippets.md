---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8ff771756ea3175d7e85653fddb017c6513a5a27
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35318652"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/synchronization/templates"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationTemplate *synchronizationTemplate = [[MSGraphSynchronizationTemplate alloc] init];
[synchronizationTemplate setId:@"SCIM-Test1"];
[synchronizationTemplate setApplicationId:@"{id}"];
[synchronizationTemplate setFactoryTag:@"CustomSCIM"];

NSError *error;
NSData *synchronizationTemplateData = [synchronizationTemplate getSerializedDataWithError:&error];
[urlRequest setHTTPBody:synchronizationTemplateData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```