---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84de55f4a87f6baad7986aa769257be5e048861b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211928"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/communications/calls"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCall *call = [[MSGraphCall alloc] init];
[call setCallbackUri:@"https://bot.contoso.com/callback"];
NSMutableArray *requestedModalitiesList = [[NSMutableArray alloc] init];
[requestedModalitiesList addObject: @"audio"];
[call setRequestedModalities:requestedModalitiesList];
MSGraphMediaConfig *mediaConfig = [[MSGraphMediaConfig alloc] init];
NSMutableArray *preFetchMediaList = [[NSMutableArray alloc] init];
MSGraphMediaInfo *preFetchMedia = [[MSGraphMediaInfo alloc] init];
[preFetchMedia setUri:@"https://cdn.contoso.com/beep.wav"];
[preFetchMedia setResourceId:@"f8971b04-b53e-418c-9222-c82ce681a582"];
[preFetchMediaList addObject: preFetchMedia];
MSGraphMediaInfo *preFetchMedia = [[MSGraphMediaInfo alloc] init];
[preFetchMedia setUri:@"https://cdn.contoso.com/cool.wav"];
[preFetchMedia setResourceId:@"86dc814b-c172-4428-9112-60f8ecae1edb"];
[preFetchMediaList addObject: preFetchMedia];
[mediaConfig setPreFetchMedia:preFetchMediaList];
[call setMediaConfig:mediaConfig];
MSGraphChatInfo *chatInfo = [[MSGraphChatInfo alloc] init];
[chatInfo setThreadId:@"19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2"];
[chatInfo setMessageId:@"0"];
[call setChatInfo:chatInfo];
MSGraphMeetingInfo *meetingInfo = [[MSGraphMeetingInfo alloc] init];
MSGraphIdentitySet *organizer = [[MSGraphIdentitySet alloc] init];
MSGraphIdentity *user = [[MSGraphIdentity alloc] init];
[user setId:@"5810cede-f3cc-42eb-b2c1-e9bd5d53ec96"];
[user setTenantId:@"aa67bd4c-8475-432d-bd41-39f255720e0a"];
[user setDisplayName:@"Bob"];
[organizer setUser:user];
[meetingInfo setOrganizer:organizer];
[meetingInfo setAllowConversationWithoutHost: true];
[call setMeetingInfo:meetingInfo];
[call setTenantId:@"86dc81db-c112-4228-9222-63f3esaa1edb"];

NSError *error;
NSData *callData = [call getSerializedDataWithError:&error];
[urlRequest setHTTPBody:callData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```