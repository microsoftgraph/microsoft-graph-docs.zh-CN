---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b0d9ac584ba6950fb4bf232c354cbec7d7b0f95b58d763a4524568cf821c947
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328713"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *recipientsList = [[NSMutableArray alloc] init];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipients setEmail:@"ryan@contoso.org"];
[recipientsList addObject: recipients];
payloadDictionary[@"recipients"] = recipientsList;

NSString *message = @"Here's the file that we're collaborating on.";
payloadDictionary[@"message"] = message;

BOOL requireSignIn = YES;
payloadDictionary[@"requireSignIn"] = requireSignIn;

BOOL sendInvitation = YES;
payloadDictionary[@"sendInvitation"] = sendInvitation;

NSMutableArray *rolesList = [[NSMutableArray alloc] init];
[rolesList addObject: @"write"];
payloadDictionary[@"roles"] = rolesList;

NSString *password = @"password123";
payloadDictionary[@"password"] = password;

NSString *expirationDateTimeDateTimeString = @"07/15/2018 14:00:00";
NSDate *expirationDateTime = [NSDate ms_dateFromString: expirationDateTimeDateTimeString];
payloadDictionary[@"expirationDateTime"] = expirationDateTime;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```