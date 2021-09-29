---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0232ef0fac428d2acbacbda8f95ca31cb1fb1bd7
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995464"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphOrganizationalBrandingLocalization *organizationalBrandingLocalization = [[MSGraphOrganizationalBrandingLocalization alloc] init];
[organizationalBrandingLocalization setBackgroundColor:@"#00000F"];
[organizationalBrandingLocalization setId:@"fr-FR"];
[organizationalBrandingLocalization setSignInPageText:@" "];

NSError *error;
NSData *organizationalBrandingLocalizationData = [organizationalBrandingLocalization getSerializedDataWithError:&error];
[urlRequest setHTTPBody:organizationalBrandingLocalizationData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```