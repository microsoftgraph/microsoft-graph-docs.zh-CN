---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec1e9b5aa34494e9017a1be479fe0bc2b157be9de6b7fc6fea7a4c9609ed5142
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279054"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/tenantRelationships/managedTenants/windowsProtectionStates/{windowsProtectionStateId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphWindowsProtectionState *windowsProtectionState = [[MSGraphWindowsProtectionState alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```