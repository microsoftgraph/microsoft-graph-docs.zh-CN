---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 715a47c1ccc7b75202d0f3d819438dab988968d3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350500"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/owners/{id}/$ref"]]];
[urlRequest setHTTPMethod:@"DELETE"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDirectoryObject *directoryObject = [[MSGraphDirectoryObject alloc] init];

NSError *error;
NSData *directoryObjectData = [directoryObject getSerializedDataWithError:&error];
[urlRequest setHTTPBody:directoryObjectData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```