---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3d4ac190e508c1d07e8351bffe51011e631e2583
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878655"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/agents?$expand=agentGroups"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        NSDictionary *jsonFinal = [NSJSONSerialization JSONObjectWithData:data options:0 error:&jsonError];
        NSMutableArray *onPremisesAgentList = [[NSMutableArray alloc] init];
        onPremisesAgentList = [jsonFinal valueForKey:@"value"];
        MSGraphOnPremisesAgent *onPremisesAgent = [[MSGraphOnPremisesAgent alloc] initWithDictionary:[onPremisesAgentList objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```