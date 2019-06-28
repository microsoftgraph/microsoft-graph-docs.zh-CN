---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 103d20e7a2c4fc0a927506fdbe89140fa1997a67
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35323076"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/mailFolders/inbox/messageRules"]]];
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