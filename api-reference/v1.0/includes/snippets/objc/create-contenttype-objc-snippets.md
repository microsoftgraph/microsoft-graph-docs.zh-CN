---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eaac75a40985639382e94a4f7f297926a6b5e87
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044885"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{id}/contentTypes"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphContentType *contentType = [[MSGraphContentType alloc] init];
[contentType setName:@"docSet"];
[contentType setDescription:@"custom docset"];
MSGraphContentType *base = [[MSGraphContentType alloc] init];
[base setName:@"Document Set"];
[base setId:@"0x0120D520"];
[contentType setBase:base];
[contentType setGroup:@"Document Set Content Types"];

NSError *error;
NSData *contentTypeData = [contentType getSerializedDataWithError:&error];
[urlRequest setHTTPBody:contentTypeData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```