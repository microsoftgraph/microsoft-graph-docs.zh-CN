---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9f9c5a8f7ce4b83cdb6ae4305ae33c27a45d79bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878287"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOnPremisesAgentGroup *onPremisesAgentGroup = [[MSGraphOnPremisesAgentGroup alloc] init];
[onPremisesAgentGroup setDisplayName:@"Group New Name"];

NSError *error;
NSData *onPremisesAgentGroupData = [onPremisesAgentGroup getSerializedDataWithError:&error];
[urlRequest setHTTPBody:onPremisesAgentGroupData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```