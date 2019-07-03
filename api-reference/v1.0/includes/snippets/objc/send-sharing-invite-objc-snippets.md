---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 463f6fe5eb0144a9c100b051f8ca6b1a5ba93c8e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467381"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/invite"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *recipientsList = [[NSMutableArray alloc] init];
MSGraphDriveRecipient *recipients = [[MSGraphDriveRecipient alloc] init];
[recipients setEmail:@"ryan@contoso.com"];
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

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```