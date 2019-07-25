---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2d92eb879e7efc0646c2b5616a4570d61b7e113f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708935"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/app/calls/{id}/audioRoutingGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *AudioRoutingGroupList = [[NSMutableArray alloc] init];
        AudioRoutingGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphAudioRoutingGroup *AudioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] initWithDictionary:[AudioRoutingGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```