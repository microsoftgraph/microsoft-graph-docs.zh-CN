---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 914a9d464a8979108fed0dbfe8ed63b039853552
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49843681"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{team-id}/channels/{channel-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChannel *channel = [[MSGraphChannel alloc] init];
[channel setDisplayName:@"UpdateChannelModeration"];
[channel setDescription:@"Update channel moderation."];
MSGraphChannelModerationSettings *moderationSettings = [[MSGraphChannelModerationSettings alloc] init];
[moderationSettings setUserNewMessageRestriction: [MSGraphUserNewMessageRestriction moderators]];
[moderationSettings setReplyRestriction: [MSGraphReplyRestriction everyone]];
[moderationSettings setAllowNewMessageFromBots: true];
[moderationSettings setAllowNewMessageFromConnectors: true];
[channel setModerationSettings:moderationSettings];

NSError *error;
NSData *channelData = [channel getSerializedDataWithError:&error];
[urlRequest setHTTPBody:channelData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```