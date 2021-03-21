---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd0093b3627c16214a77d6911bab45f194873475
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964316"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/teams/{id}/channels/{id}/messages"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphChatMessage *chatMessage = [[MSGraphChatMessage alloc] init];
MSGraphItemBody *body = [[MSGraphItemBody alloc] init];
[body setContentType: [MSGraphBodyType html]];
[body setContent:@"Here's the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>"];
[chatMessage setBody:body];
NSMutableArray *attachmentsList = [[NSMutableArray alloc] init];
MSGraphChatMessageAttachment *attachments = [[MSGraphChatMessageAttachment alloc] init];
[attachments setId:@"153fa47d-18c9-4179-be08-9879815a9f90"];
[attachments setContentType:@"reference"];
[attachments setContentUrl:@"https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx"];
[attachments setName:@"Budget.docx"];
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