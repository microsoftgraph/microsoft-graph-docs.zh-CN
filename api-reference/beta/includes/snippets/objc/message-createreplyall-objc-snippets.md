---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc88d9c46718732d700eb2db56c92527ae13ff61c888dbea027b3a14ef6a212e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220639"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/AAMkADA1MTAAAH5JaKAAA=/createReplyAll"]]];
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

NSString *comment = @"if the project gets approved, please take a look at the attached guidelines before you decide on the name.";
payloadDictionary[@"comment"] = comment;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```