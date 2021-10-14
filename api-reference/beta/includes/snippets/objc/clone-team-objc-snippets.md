---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75c900b62409d37f5425bfb0f692757446f3ab79aa2ca7a6cc593c36fa5fbf48
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903922"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/clone"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *displayName = @"Library Assist";
payloadDictionary[@"displayName"] = displayName;

NSString *description = @"Self help community for library";
payloadDictionary[@"description"] = description;

NSString *mailNickname = @"libassist";
payloadDictionary[@"mailNickname"] = mailNickname;

MSGraphClonableTeamParts *partsToClone = [MSGraphClonableTeamParts apps];
payloadDictionary[@"partsToClone"] = partsToClone;

MSGraphTeamVisibilityType *visibility = [MSGraphTeamVisibilityType public];
payloadDictionary[@"visibility"] = visibility;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```