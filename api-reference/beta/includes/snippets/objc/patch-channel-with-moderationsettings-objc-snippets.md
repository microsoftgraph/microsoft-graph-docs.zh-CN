---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 498c42015b988b61ded4bbe8643dbc380361d805
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509015"
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