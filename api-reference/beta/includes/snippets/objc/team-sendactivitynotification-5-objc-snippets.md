---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94a4444365f8f0741c61d2b301916723e76d5c6a7bd1413e14edaec48cf33323
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163368"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7/sendActivityNotification"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphTeamworkActivityTopic *topic = [[MSGraphTeamworkActivityTopic alloc] init];
[topic setSource: [MSGraphTeamworkActivityTopicSource entityUrl]];
[topic setValue:@"https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7"];
payloadDictionary[@"topic"] = topic;

NSString *activityType = @"pendingFinanceApprovalRequests";
payloadDictionary[@"activityType"] = activityType;

MSGraphItemBody *previewText = [[MSGraphItemBody alloc] init];
[previewText setContent:@"Internal spending team has a pending finance approval requests"];
payloadDictionary[@"previewText"] = previewText;

MSGraphTeamworkNotificationRecipient *recipient = [[MSGraphTeamworkNotificationRecipient alloc] init];
[recipient setTeamId:@"e8bece96-d393-4b9b-b8da-69cedef1a7e7"];
[recipient setChannelId:@"19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"];
payloadDictionary[@"recipient"] = recipient;

NSMutableArray *templateParametersList = [[NSMutableArray alloc] init];
MSGraphKeyValuePair *templateParameters = [[MSGraphKeyValuePair alloc] init];
[templateParameters setName:@"pendingRequestCount"];
[templateParameters setValue:@"5"];
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