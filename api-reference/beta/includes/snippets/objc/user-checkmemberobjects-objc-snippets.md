---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c063b41ec40c47316806cda2bc9cede43aa662a054052bd9628a3942e210c71
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105702"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me/checkMemberObjects"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSMutableArray *idsList = [[NSMutableArray alloc] init];
[idsList addObject: @"80a963dd-84af-4eb8-b2a6-781e444d4fb0"];
[idsList addObject: @"62e90394-69f5-4237-9190-012177145e10"];
[idsList addObject: @"86a64f51-3a64-4cc6-a8c8-6b8f000c0f52"];
[idsList addObject: @"ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"];
payloadDictionary[@"ids"] = idsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```