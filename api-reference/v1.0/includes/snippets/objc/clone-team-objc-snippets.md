---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 045d36a221c3a353c7de4046983c832a0d615830
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335696"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
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