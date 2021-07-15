---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24b5d36f319e72547459898ec153df332d47e65d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440696"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/entitlementManagement/roleDefinitions/ba92d953-d8e0-4e39-a797-0cbedb0a89e8"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleDefinition *unifiedRoleDefinition = [[MSGraphUnifiedRoleDefinition alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```