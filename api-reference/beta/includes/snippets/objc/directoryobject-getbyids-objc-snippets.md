---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a0e0e2de2bcc6f7da035aea41bd7ed2d7203ca1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706737"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryObjects/getByIds"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *idsList = [[NSMutableArray alloc] init];
[idsList addObject: @"84b80893-8749-40a3-97b7-68513b600544"];
[idsList addObject: @"5d6059b6-368d-45f8-91e1-8e07d485f1d0"];
payloadDictionary[@"ids"] = idsList;

NSMutableArray *typesList = [[NSMutableArray alloc] init];
[typesList addObject: @"user"];
payloadDictionary[@"types"] = typesList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```