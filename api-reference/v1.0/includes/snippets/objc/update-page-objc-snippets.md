---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa66e5c8a70941f4f6eb8387f3a9acc44eb93a74
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428781"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/onenote/pages/{id}/content"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableArray *streamList = [[NSMutableArray alloc] init];
MSGraphStream *stream = [[MSGraphStream alloc] init];
[stream setTarget:@"#para-id"];
[stream setAction:@"insert"];
[stream setPosition:@"before"];
[stream setContent:@"<img src=\"image-url-or-part-name\" alt=\"image-alt-text\" />"];
[streamList addObject: stream];
MSGraphStream *stream = [[MSGraphStream alloc] init];
[stream setTarget:@"#list-id"];
[stream setAction:@"append"];
[stream setContent:@"<li>new-page-content</li>"];
[streamList addObject: stream];

NSError *error;
NSData *streamData = [stream getSerializedDataWithError:&error];
[urlRequest setHTTPBody:streamData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```