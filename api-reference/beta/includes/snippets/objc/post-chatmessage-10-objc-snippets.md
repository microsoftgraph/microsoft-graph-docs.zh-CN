---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 523b3644b954f0a63ab7f2e50ce93eecf6a8f971
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208936"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
[chatMessage setSubject: null];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>"];
[chatMessage setBody:body];
NSMutableArray *attachmentsList = [[NSMutableArray alloc] init];
MSGraphChatMessageAttachment *attachments = [[MSGraphChatMessageAttachment alloc] init];
[attachments setId:@"74d20c7f34aa4a7fb74e2b30004247c5"];
[attachments setContentType:@"application/vnd.microsoft.card.thumbnail"];
[attachments setContentUrl: null];
[attachments setContent:@"{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\\r\\nAnd a <a href=\\\"http://microsoft.com/\\\">hyperlink</a>. <br>\\r\\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}"];
[attachments setName: null];
[attachments setThumbnailUrl: null];
[attachments setTeamsAppId:@"881b8843-fd91-49e5-9ac2-47ec497ffbe5"];
[attachmentsList addObject: attachments];
[chatMessage setAttachments:attachmentsList];

NSError *error;
NSData *chatMessageData = [chatMessage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:chatMessageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```