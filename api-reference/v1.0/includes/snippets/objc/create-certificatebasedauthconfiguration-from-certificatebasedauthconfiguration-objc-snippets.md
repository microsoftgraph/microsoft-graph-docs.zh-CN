---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b799de9d9bf20c190389fb92a5debd4ceb94dee3
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905797"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/{id}/certificateBasedAuthConfiguration/$ref"]]];
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