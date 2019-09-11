---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ded9f578801c903825a9772afad0e0e2c806718f
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36839071"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/root/workbook/comments/{id}/replies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphWorkbookCommentReply *workbookCommentReply = [[MSGraphWorkbookCommentReply alloc] init];
[workbookCommentReply setContent:@"This is my reply to the comment."];
[workbookCommentReply setContentType:@"plain"];

NSError *error;
NSData *workbookCommentReplyData = [workbookCommentReply getSerializedDataWithError:&error];
[urlRequest setHTTPBody:workbookCommentReplyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```