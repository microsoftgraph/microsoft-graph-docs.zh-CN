---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c21809742b4136d02bace064285220b2938bb094
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933828"
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
        NSMutableArray *audioRoutingGroupList = [[NSMutableArray alloc] init];
        audioRoutingGroupList = [jsonFinal valueForKey:@"value"];
        MSGraphAudioRoutingGroup *audioRoutingGroup = [[MSGraphAudioRoutingGroup alloc] initWithDictionary:[audioRoutingGroupList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```