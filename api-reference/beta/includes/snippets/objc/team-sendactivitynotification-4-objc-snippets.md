---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8769646ede5f243cb3d50e207abe3044d6beaeaabdff1800736ab349e6a1eeef
ms.sourcegitcommit: 24d0ea8e2bcb54c2f397133460c3d26fb0ba705f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "58785463"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/users/{userId}/teamwork/sendActivityNotification"]]];
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