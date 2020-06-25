---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a56ec92686900f20465bbbe9da0837b7cfad2bc
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44866544"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/{id}/team"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTeam *team = [[MSGraphTeam alloc] init];
MSGraphTeamMemberSettings *memberSettings = [[MSGraphTeamMemberSettings alloc] init];
[memberSettings setAllowCreatePrivateChannels: true];
[memberSettings setAllowCreateUpdateChannels: true];
[team setMemberSettings:memberSettings];
MSGraphTeamMessagingSettings *messagingSettings = [[MSGraphTeamMessagingSettings alloc] init];
[messagingSettings setAllowUserEditMessages: true];
[messagingSettings setAllowUserDeleteMessages: true];
[team setMessagingSettings:messagingSettings];
MSGraphTeamFunSettings *funSettings = [[MSGraphTeamFunSettings alloc] init];
[funSettings setAllowGiphy: true];
[funSettings setGiphyContentRating: [MSGraphGiphyRatingType strict]];
[team setFunSettings:funSettings];

NSError *error;
NSData *teamData = [team getSerializedDataWithError:&error];
[urlRequest setHTTPBody:teamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```