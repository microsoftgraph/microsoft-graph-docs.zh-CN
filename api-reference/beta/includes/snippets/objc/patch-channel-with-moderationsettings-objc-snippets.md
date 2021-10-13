---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91d149a4fb117eef6ce196ec64cbf223c1de07b2529b510ba4882a5f4127b6e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902440"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/893075dd-2487-4122-925f-022c42e20265/channels/19:561fbdbbfca848a484f0a6f00ce9dbbd@thread.tacv2"]]];
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