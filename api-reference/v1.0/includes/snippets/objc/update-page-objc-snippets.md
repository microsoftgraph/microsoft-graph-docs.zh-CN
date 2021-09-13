---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 633baf21457c717026dc15c2bf85beaaef882528f6ed71721d619feaf1c46c9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333924"
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