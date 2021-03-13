---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc0fc1f8275a7ab001eb191926d06ce3bc3bb511
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773338"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphColumnDefinition *columnDefinition = [[MSGraphColumnDefinition alloc] init];
[columnDefinition setRequired: true];
[columnDefinition setHidden: false];
[columnDefinition setPropagateChanges: false];

NSError *error;
NSData *columnDefinitionData = [columnDefinition getSerializedDataWithError:&error];
[urlRequest setHTTPBody:columnDefinitionData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```