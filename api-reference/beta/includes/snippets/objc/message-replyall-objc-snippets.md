---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 59b626fa629da8a486cbe4a8ccc3fcb6ae8f7c1b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729552"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphMessage *message = [[MSGraphMessage alloc] init];
NSMutableArray *attachmentsList = [[NSMutableArray alloc] init];
MSGraphAttachment *attachments = [[MSGraphAttachment alloc] init];
[attachments setName:@"guidelines.txt"];
[attachments setContentBytes:@"bWFjIGFuZCBjaGVlc2UgdG9kYXk="];
[attachmentsList addObject: attachments];
[message setAttachments:attachmentsList];
payloadDictionary[@"message"] = message;

NSString *comment = @"Please take a look at the attached guidelines before you decide on the name.";
payloadDictionary[@"comment"] = comment;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```