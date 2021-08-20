---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8d50361b7d8b6a0fedec8b77bc8645d65533b5bb9146a9c1cda6062300d1507
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903183"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/reports/authenticationMethods/usersRegisteredByFeature(includedUserTypes='all',includedUserRoles='all')"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUserRegistrationFeatureSummary *userRegistrationFeatureSummary = [[MSGraphUserRegistrationFeatureSummary alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```