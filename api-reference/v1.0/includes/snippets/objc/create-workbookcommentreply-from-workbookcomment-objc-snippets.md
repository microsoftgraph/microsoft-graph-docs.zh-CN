---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ba181f06c675e1dae4daa3185d9053ca5b701fa
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41497766"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/drive/items/{id}/workbook/comments/{id}/replies"]]];
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