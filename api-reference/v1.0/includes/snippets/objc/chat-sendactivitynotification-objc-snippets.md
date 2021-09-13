---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1014f6d32ec0d734fc4e3380c4e41258669a252d9682daf6160e55ff4c3b37d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163524"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/chats/{chatId}/sendActivityNotification"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphTeamworkActivityTopic *topic = [[MSGraphTeamworkActivityTopic alloc] init];
[topic setSource: [MSGraphTeamworkActivityTopicSource text]];
[topic setValue:@"Deployment Approvals Channel"];
[topic setWebUrl:@"https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"];
payloadDictionary[@"topic"] = topic;

NSString *activityType = @"deploymentApprovalRequired";
payloadDictionary[@"activityType"] = activityType;

MSGraphItemBody *previewText = [[MSGraphItemBody alloc] init];
[previewText setContent:@"New deployment requires your approval"];
payloadDictionary[@"previewText"] = previewText;

MSGraphTeamworkNotificationRecipient *recipient = [[MSGraphTeamworkNotificationRecipient alloc] init];
[recipient setUserId:@"569363e2-4e49-4661-87f2-16f245c5d66a"];
payloadDictionary[@"recipient"] = recipient;

NSMutableArray *templateParametersList = [[NSMutableArray alloc] init];
MSGraphKeyValuePair *templateParameters = [[MSGraphKeyValuePair alloc] init];
[templateParameters setName:@"deploymentId"];
[templateParameters setValue:@"6788662"];
[templateParametersList addObject: templateParameters];
payloadDictionary[@"templateParameters"] = templateParametersList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```