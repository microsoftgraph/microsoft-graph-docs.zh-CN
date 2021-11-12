---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a60d81063c9f87c2cf0b386023422a14c1d204802c1153b6696cda7b3cfa7fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278675"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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