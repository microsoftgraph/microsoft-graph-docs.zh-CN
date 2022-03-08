---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccc88408fb5665727ecfbc3ac3592e62644827b1e32f4a0bacbcbc482282e935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104496"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration?$expand=postFederationSignup,postAttributeCollection"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUserFlowApiConnectorConfiguration *userFlowApiConnectorConfiguration = [[MSGraphUserFlowApiConnectorConfiguration alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```