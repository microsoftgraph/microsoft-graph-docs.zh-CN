---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0de43059b425e03a69e290729c47e14cc4fad6fa
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638653"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{id}/certificateBasedAuthConfiguration"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphCertificateBasedAuthConfiguration *certificateBasedAuthConfiguration = [[MSGraphCertificateBasedAuthConfiguration alloc] init];
NSMutableArray *certificateAuthoritiesList = [[NSMutableArray alloc] init];
MSGraphCertificateAuthority *certificateAuthorities = [[MSGraphCertificateAuthority alloc] init];
[certificateAuthorities setIsRootAuthority: true];
[certificateAuthorities setCertificate:@"Binary"];
[certificateAuthoritiesList addObject: certificateAuthorities];
[certificateBasedAuthConfiguration setCertificateAuthorities:certificateAuthoritiesList];

NSError *error;
NSData *certificateBasedAuthConfigurationData = [certificateBasedAuthConfiguration getSerializedDataWithError:&error];
[urlRequest setHTTPBody:certificateBasedAuthConfigurationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```