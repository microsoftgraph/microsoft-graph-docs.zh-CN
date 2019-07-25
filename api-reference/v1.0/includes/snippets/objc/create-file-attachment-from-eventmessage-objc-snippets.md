---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26f7279fa5257c0c390815552feca4143460ef2e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731647"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/messages/{id}/attachments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAttachment *attachment = [[MSGraphAttachment alloc] init];
[attachment setName:@"name-value"];
[attachment setContentType:@"contentType-value"];
[attachment setIsInline: false];
[attachment setContentLocation:@"contentLocation-value"];
[attachment setContentBytes:@"base64-contentBytes-value"];

NSError *error;
NSData *attachmentData = [attachment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:attachmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```