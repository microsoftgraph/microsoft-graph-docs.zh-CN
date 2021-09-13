---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37cb33b5bd7eebf611d1c681cc518e7789e3178bb075fb85ff5b165e955045b7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162884"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphIdentityUserFlowAttributeAssignment *identityUserFlowAttributeAssignment = [[MSGraphIdentityUserFlowAttributeAssignment alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```