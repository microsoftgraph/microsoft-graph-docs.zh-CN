---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed5ccfe56125a8385b42b008ce48e7fd388148702aac0861b01ee12f7eba3f5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158708"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/directoryObjects/getByIds"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *idsList = [[NSMutableArray alloc] init];
[idsList addObject: @"84b80893874940a3-97b7-68513b600544"];
[idsList addObject: @"5d6059b6368d-45f8-91e18e07d485f1d0"];
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