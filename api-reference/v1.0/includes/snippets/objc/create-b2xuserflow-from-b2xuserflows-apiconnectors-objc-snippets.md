---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1eaf08b4b0ada1a08038d7244754b4e3a7de68582a128e6f1f2d2bcacf130ca2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220420"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphB2xIdentityUserFlow *b2xIdentityUserFlow = [[MSGraphB2xIdentityUserFlow alloc] init];
[b2xIdentityUserFlow setId:@"UserFlowWithAPIConnector"];
[b2xIdentityUserFlow setUserFlowType: [MSGraphUserFlowType signUpOrSignIn]];
[b2xIdentityUserFlow setUserFlowTypeVersion: 1];
MSGraphUserFlowApiConnectorConfiguration *apiConnectorConfiguration = [[MSGraphUserFlowApiConnectorConfiguration alloc] init];
MSGraphIdentityApiConnector *postFederationSignup = [[MSGraphIdentityApiConnector alloc] init];
[apiConnectorConfiguration setPostFederationSignup:postFederationSignup];
MSGraphIdentityApiConnector *postAttributeCollection = [[MSGraphIdentityApiConnector alloc] init];
[apiConnectorConfiguration setPostAttributeCollection:postAttributeCollection];
[b2xIdentityUserFlow setApiConnectorConfiguration:apiConnectorConfiguration];

NSError *error;
NSData *b2xIdentityUserFlowData = [b2xIdentityUserFlow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2xIdentityUserFlowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```