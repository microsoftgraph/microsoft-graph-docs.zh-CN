---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7914e91e5f5ccfb5c6bda027ea88147a49f9e62aa9bf2f6bad8870d4169dc8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409001"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/security/secureScoreControlProfiles/NonOwnerAccess"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphSecureScoreControlProfile *secureScoreControlProfile = [[MSGraphSecureScoreControlProfile alloc] init];
[secureScoreControlProfile setAssignedTo:@""];
[secureScoreControlProfile setComment:@"control is reviewed"];
[secureScoreControlProfile setState:@"Reviewed"];
MSGraphSecurityVendorInformation *vendorInformation = [[MSGraphSecurityVendorInformation alloc] init];
[vendorInformation setProvider:@"SecureScore"];
[vendorInformation setProviderVersion: null];
[vendorInformation setSubProvider: null];
[vendorInformation setVendor:@"Microsoft"];
[secureScoreControlProfile setVendorInformation:vendorInformation];

NSError *error;
NSData *secureScoreControlProfileData = [secureScoreControlProfile getSerializedDataWithError:&error];
[urlRequest setHTTPBody:secureScoreControlProfileData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```