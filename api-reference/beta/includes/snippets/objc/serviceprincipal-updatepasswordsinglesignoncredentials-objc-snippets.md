---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aad6e5d6c8f07b0885da61c794035f55a17c984b8e1eb899698bff1eb06e199b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273843"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/updatePasswordSingleSignOnCredentials"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

NSMutableDictionary *payloadDictionary = [[NSMutableDictionary alloc] init];

NSString *id = @"5793aa3b-cca9-4794-679a240f8b58";
payloadDictionary[@"id"] = id;

NSMutableArray *credentialsList = [[NSMutableArray alloc] init];
MSGraphCredential *credentials = [[MSGraphCredential alloc] init];
[credentials setFieldId:@"param_username"];
[credentials setValue:@"myusername"];
[credentials setType:@"username"];
[credentialsList addObject: credentials];
MSGraphCredential *credentials = [[MSGraphCredential alloc] init];
[credentials setFieldId:@"param_password"];
[credentials setValue:@"pa$$w0rd"];
[credentials setType:@"password"];
[credentialsList addObject: credentials];
payloadDictionary[@"credentials"] = credentialsList;

NSData *data = [NSJSONSerialization dataWithJSONObject:payloadDictionary options:kNilOptions error:&error];
[urlRequest setHTTPBody:data];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```