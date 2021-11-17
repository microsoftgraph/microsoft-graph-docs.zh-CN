---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17285cc028b98a5879b78e2b4a20f6e7b764a907d8f3c82030e810d6edca009b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902497"
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