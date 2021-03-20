---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30a2c0b0edb103bfa3c87497692bc10d2e0ebd32
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944353"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/informationProtection/bitlocker/recoveryKeys?$filter=deviceId%20eq%20'1ab40ab2-32a8-4b00-b6b5-ba724e407de9'"]]];
[urlRequest setHTTPMethod:@"GET"];
[urlRequest setValue:@"\"My Friendly Client\"" forHTTPHeaderField:@"ocp-client-name"];
[urlRequest setValue:@"\"1.2\"" forHTTPHeaderField:@"ocp-client-version"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        NSError *jsonError = nil;
        MSCollection *collection = [[MSCollection alloc] initWithData:data error:&jsonError];
        MSGraphBitlockerRecoveryKey *bitlockerRecoveryKey = [[MSGraphBitlockerRecoveryKey alloc] initWithDictionary:[[collection value] objectAtIndex: 0] error:&nserror];

}];

[meDataTask execute];

```