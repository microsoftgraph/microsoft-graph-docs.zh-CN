---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94106ad5db69c9c123d387fc0b3289757e77c85c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905150"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/addKey"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

MSGraphKeyCredential *keyCredential = [[MSGraphKeyCredential alloc] init];
[keyCredential setType:@"X509CertAndPassword"];
[keyCredential setUsage:@"Sign"];
[keyCredential setKey:@"MIIDYDCCAki..."];
payloadDictionary[@"keyCredential"] = keyCredential;

MSGraphPasswordCredential *passwordCredential = [[MSGraphPasswordCredential alloc] init];
[passwordCredential setSecretText:@"MKTr0w1..."];
payloadDictionary[@"passwordCredential"] = passwordCredential;

NSString *proof = @"eyJ0eXAiOiJ...";
payloadDictionary[@"proof"] = proof;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```