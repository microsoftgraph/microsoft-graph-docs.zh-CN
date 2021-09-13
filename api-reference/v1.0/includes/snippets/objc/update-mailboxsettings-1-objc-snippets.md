---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c57c5d4a8959d196a79a4aefb153f7a3f37d3449f696bd72ad7474b306b8e47f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218373"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailboxSettings"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMailboxSettings *mailboxSettings = [[MSGraphMailboxSettings alloc] init];
MSGraphAutomaticRepliesSetting *automaticRepliesSetting = [[MSGraphAutomaticRepliesSetting alloc] init];
[automaticRepliesSetting setStatus: [MSGraphAutomaticRepliesStatus scheduled]];
MSGraphDateTimeTimeZone *scheduledStartDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[scheduledStartDateTime setDateTime: "2016-03-20T18:00:00"];
[scheduledStartDateTime setTimeZone:@"UTC"];
[automaticRepliesSetting setScheduledStartDateTime:scheduledStartDateTime];
MSGraphDateTimeTimeZone *scheduledEndDateTime = [[MSGraphDateTimeTimeZone alloc] init];
[scheduledEndDateTime setDateTime: "2016-03-28T18:00:00"];
[scheduledEndDateTime setTimeZone:@"UTC"];
[automaticRepliesSetting setScheduledEndDateTime:scheduledEndDateTime];
[mailboxSettings setAutomaticRepliesSetting:automaticRepliesSetting];

NSError *error;
NSData *mailboxSettingsData = [mailboxSettings getSerializedDataWithError:&error];
[urlRequest setHTTPBody:mailboxSettingsData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```