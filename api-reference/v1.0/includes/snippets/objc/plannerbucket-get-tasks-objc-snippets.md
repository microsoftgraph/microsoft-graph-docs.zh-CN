---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1751f4fadf4e143752278530c8692e490f817aa3
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123106"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/planner/buckets/{bucket-id}/tasks"]]];
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