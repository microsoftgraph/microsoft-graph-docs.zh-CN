---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: daf1a62c199428eb296e28cb3604c9abcfbb59e2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616785"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/devices"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphDevice *device = [[MSGraphDevice alloc] init];
[device setAccountEnabled: true];
NSMutableArray *alternativeSecurityIdsList = [[NSMutableArray alloc] init];
MSGraphAlternativeSecurityId *alternativeSecurityIds = [[MSGraphAlternativeSecurityId alloc] init];
[alternativeSecurityIds setType: 99];
[alternativeSecurityIds setIdentityProvider:@"identityProvider-value"];
[alternativeSecurityIds setKey:@"base64Y3YxN2E1MWFlYw=="];
[alternativeSecurityIdsList addObject: alternativeSecurityIds];
[device setAlternativeSecurityIds:alternativeSecurityIdsList];
[device setApproximateLastSignInDateTime: "2016-10-19T10:37:00Z"];
[device setDeviceId:@"deviceId-value"];
[device setDeviceMetadata:@"deviceMetadata-value"];
[device setDeviceVersion: 99];

NSError *error;
NSData *deviceData = [device getSerializedDataWithError:&error];
[urlRequest setHTTPBody:deviceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```