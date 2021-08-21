---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95e05b97b5359064d6933956bd14765d53f03c6c000e6db619ab6f0058bc858b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903795"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphGovernanceRoleSetting *governanceRoleSetting = [[MSGraphGovernanceRoleSetting alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```