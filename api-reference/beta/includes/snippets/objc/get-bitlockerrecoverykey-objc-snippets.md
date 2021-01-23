---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1393cb76a2a0f04f54727e35d1e39780cdce1de
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944908"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/bitlocker/recoveryKeys?$filter=deviceId%20eq%20'1ab40ab2-32a8-4b00-b6b5-ba724e407de9'"]]];
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