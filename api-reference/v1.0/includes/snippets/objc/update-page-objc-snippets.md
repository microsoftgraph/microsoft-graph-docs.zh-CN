---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 28c9f93818a5cf9e34ccc3a6de4f6c55b9380fec
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466857"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/pages/{id}/content"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableArray *StreamList = [[NSMutableArray alloc] init];
MSGraphStream *Stream = [[MSGraphStream alloc] init];
[Stream setTarget:@"#para-id"];
[Stream setAction:@"insert"];
[Stream setPosition:@"before"];
[Stream setContent:@"<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />"];
[StreamList addObject: Stream];
MSGraphStream *Stream = [[MSGraphStream alloc] init];
[Stream setTarget:@"#list-id"];
[Stream setAction:@"append"];
[Stream setContent:@"<li>new-page-content</li>"];
[StreamList addObject: Stream];

NSError *error;
NSData *StreamData = [Stream getSerializedDataWithError:&error];
[urlRequest setHTTPBody:StreamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```