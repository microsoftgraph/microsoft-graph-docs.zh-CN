---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cba3165f00128b933cafabe96da55222e16ac17
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690108"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/servicePrincipals/{id}/appManagementPolicies/$ref"]]];
[urlRequest setHTTPMethod:@"POST"];

MSGraphAppManagementPolicy *appManagementPolicy = [[MSGraphAppManagementPolicy alloc] init];

NSError *error;
NSData *appManagementPolicyData = [appManagementPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:appManagementPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```