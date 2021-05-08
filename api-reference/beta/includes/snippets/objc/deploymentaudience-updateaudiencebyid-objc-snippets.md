---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fdcd61b921a5ca9d407eb2d88f1fffc87e2b349
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240575"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *memberEntityType = @"String";
payloadDictionary[@"memberEntityType"] = memberEntityType;

NSMutableArray *addMembersList = [[NSMutableArray alloc] init];
[addMembersList addObject: @"String"];
payloadDictionary[@"addMembers"] = addMembersList;

NSMutableArray *removeMembersList = [[NSMutableArray alloc] init];
[removeMembersList addObject: @"String"];
payloadDictionary[@"removeMembers"] = removeMembersList;

NSMutableArray *addExclusionsList = [[NSMutableArray alloc] init];
[addExclusionsList addObject: @"String"];
payloadDictionary[@"addExclusions"] = addExclusionsList;

NSMutableArray *removeExclusionsList = [[NSMutableArray alloc] init];
[removeExclusionsList addObject: @"String"];
payloadDictionary[@"removeExclusions"] = removeExclusionsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```