---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88608ae7f8d8c25af8d3704d9cc7e78bec5abf98
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949345"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOrganizationalBranding *organizationalBranding = [[MSGraphOrganizationalBranding alloc] init];
[organizationalBranding setSignInPageText:@"Default"];
[organizationalBranding setUsernameHintText:@"DefaultHint"];

NSError *error;
NSData *organizationalBrandingData = [organizationalBranding getSerializedDataWithError:&error];
[urlRequest setHTTPBody:organizationalBrandingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```