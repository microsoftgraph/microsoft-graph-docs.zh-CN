---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f901e201911991e7b990d4a6ea28c56d8aab1262b5d9ffdcf779b0ab6f53634b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333245"
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