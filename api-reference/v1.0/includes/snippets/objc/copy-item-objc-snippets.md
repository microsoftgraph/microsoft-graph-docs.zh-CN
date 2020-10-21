---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 294b2c38cedf7052c7bf8a944c4dd7947d0492ab
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608093"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/drive/items/{item-id}/copy"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphItemReference *parentReference = [[MSGraphItemReference alloc] init];
[parentReference setDriveId:@"6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B"];
[parentReference setId:@"DCD0D3AD-8989-4F23-A5A2-2C086050513F"];
payloadDictionary[@"parentReference"] = parentReference;

NSString *name = @"contoso plan (copy).txt";
payloadDictionary[@"name"] = name;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```