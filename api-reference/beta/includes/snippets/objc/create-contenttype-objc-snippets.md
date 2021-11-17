---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e17c56486b6476f549d37adcffb63600705e469dc97080f35500b5d93abe1af6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218444"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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