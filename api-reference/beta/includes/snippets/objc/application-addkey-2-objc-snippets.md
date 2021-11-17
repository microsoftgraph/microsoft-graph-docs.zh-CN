---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea9fc9546ec0a37194afc9bc749d4c85b6c6fc55f8b0c72a2afb6023315ea0e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215687"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/{id}/addKey"]]];
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