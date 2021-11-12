---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b751b9e2dfd2f6c111e5775387c556aae9c792471631e4e966af10c647b90f8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218820"
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