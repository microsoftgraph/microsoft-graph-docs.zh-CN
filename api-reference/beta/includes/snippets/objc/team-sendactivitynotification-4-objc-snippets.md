---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 278e602abec134e8b7a1f07e0cb513778819df19
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317118"
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