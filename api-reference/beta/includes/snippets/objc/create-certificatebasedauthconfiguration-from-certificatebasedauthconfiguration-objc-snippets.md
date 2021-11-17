---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 741a491fe27cc2a26ecf5b4460cff5c7fbc96c09fdb2d60ef0ce823957f2de43
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274023"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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