---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c390a640c23454b30203d64b832ac4196ebd97b552c9b3e3ee594e029c4aabba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106524"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messagerules"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphMessageRule *messageRule = [[MSGraphMessageRule alloc] init];
[messageRule setDisplayName:@"From partner"];
[messageRule setSequence: 2];
[messageRule setIsEnabled: true];
MSGraphMessageRulePredicates *conditions = [[MSGraphMessageRulePredicates alloc] init];
NSMutableArray *senderContainsList = [[NSMutableArray alloc] init];
[senderContainsList addObject: @"adele"];
[conditions setSenderContains:senderContainsList];
[messageRule setConditions:conditions];
MSGraphMessageRuleActions *actions = [[MSGraphMessageRuleActions alloc] init];
NSMutableArray *forwardToList = [[NSMutableArray alloc] init];
MSGraphRecipient *forwardTo = [[MSGraphRecipient alloc] init];
MSGraphEmailAddress *emailAddress = [[MSGraphEmailAddress alloc] init];
[emailAddress setName:@"Alex Wilbur"];
[emailAddress setAddress:@"AlexW@contoso.onmicrosoft.com"];
[forwardTo setEmailAddress:emailAddress];
[forwardToList addObject: forwardTo];
[actions setForwardTo:forwardToList];
[actions setStopProcessingRules: true];
[messageRule setActions:actions];

NSError *error;
NSData *messageRuleData = [messageRule getSerializedDataWithError:&error];
[urlRequest setHTTPBody:messageRuleData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```