---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f66ba7a3135de7a9e4a3a5b0b6305496cab7b04c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37637805"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/planner/tasks"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *plannerTaskList = [[NSMutableArray alloc] init];
        plannerTaskList = [jsonFinal valueForKey:@"value"];
        MSGraphPlannerTask *plannerTask = [[MSGraphPlannerTask alloc] initWithDictionary:[plannerTaskList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```