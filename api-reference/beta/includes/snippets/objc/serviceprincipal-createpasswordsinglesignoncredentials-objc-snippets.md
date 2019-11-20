---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f44fe540368f63f24d4ec27cc391ec5878cd6a1
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747919"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/createPasswordSingleSignOnCredentials"]]];
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