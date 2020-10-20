---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad4bcdeacac41e538c5b4ebac57aa6d3e9cd11e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615518"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/synchronization/templates/{templateId}"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"Bearer <token>" forHTTPHeaderField:@"Authorization"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSynchronizationTemplate *synchronizationTemplate = [[MSGraphSynchronizationTemplate alloc] init];
[synchronizationTemplate setId:@"Slack"];
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