---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 61c5ec02b3efa8f939d2d4b22a12f7859f2baa67
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499965"
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