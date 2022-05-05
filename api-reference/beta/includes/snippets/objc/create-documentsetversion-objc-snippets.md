---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d354a26fd6fadddc42cd172719ab93b3715d92b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211501"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/root/lists/Documents/items/2/documentSetVersions"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDocumentSetVersion *documentSetVersion = [[MSGraphDocumentSetVersion alloc] init];
[documentSetVersion setComment:@"v1"];
[documentSetVersion setShouldCaptureMinorVersion: false];

NSError *error;
NSData *documentSetVersionData = [documentSetVersion getSerializedDataWithError:&error];
[urlRequest setHTTPBody:documentSetVersionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```