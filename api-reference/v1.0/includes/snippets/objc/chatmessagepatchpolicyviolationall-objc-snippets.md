---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68c3a0e60c7ed5fd8f69b255447246c67abe9a22
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315456"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19:a21b0b0c05194ebc9e30000000000f61@thread.skype"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
MSGraphChatMessagePolicyViolation *policyViolation = [[MSGraphChatMessagePolicyViolation alloc] init];
MSGraphChatMessagePolicyViolationPolicyTip *policyTip = [[MSGraphChatMessagePolicyViolationPolicyTip alloc] init];
[policyTip setGeneralText:@"This item has been blocked by the administrator."];
[policyTip setComplianceUrl:@"https://contoso.com/dlp-policy-page"];
NSMutableArray *matchedConditionDescriptionsList = [[NSMutableArray alloc] init];
[matchedConditionDescriptionsList addObject: @"Credit Card Number"];
[policyTip setMatchedConditionDescriptions:matchedConditionDescriptionsList];
[policyViolation setPolicyTip:policyTip];
[policyViolation setVerdictDetails: [MSGraphChatMessagePolicyViolationVerdictDetailsTypes allowOverrideWithoutJustification]];
[policyViolation setDlpAction: [MSGraphChatMessagePolicyViolationDlpActionTypes blockAccess]];
[chatMessage setPolicyViolation:policyViolation];

NSError *error;
NSData *chatMessageData = [chatMessage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatMessageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```