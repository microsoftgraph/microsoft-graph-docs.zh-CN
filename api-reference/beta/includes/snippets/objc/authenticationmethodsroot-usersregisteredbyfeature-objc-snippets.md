---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e4a7bd96838b539f7ead2bffa546b9dc3b321db
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092333"
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