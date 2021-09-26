---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b3202e516f7dd430780348dfe8f356f77e410bdd1e573de7292547f66b59c4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161467"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2cUserFlows"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphB2cIdentityUserFlow *b2cIdentityUserFlow = [[MSGraphB2cIdentityUserFlow alloc] init];
[b2cIdentityUserFlow setId:@"UserFlowWithAPIConnector"];
[b2cIdentityUserFlow setUserFlowType: [MSGraphUserFlowType signUpOrSignIn]];
[b2cIdentityUserFlow setUserFlowTypeVersion: 1];
MSGraphUserFlowApiConnectorConfiguration *apiConnectorConfiguration = [[MSGraphUserFlowApiConnectorConfiguration alloc] init];
MSGraphIdentityApiConnector *postFederationSignup = [[MSGraphIdentityApiConnector alloc] init];
[apiConnectorConfiguration setPostFederationSignup:postFederationSignup];
MSGraphIdentityApiConnector *postAttributeCollection = [[MSGraphIdentityApiConnector alloc] init];
[apiConnectorConfiguration setPostAttributeCollection:postAttributeCollection];
[b2cIdentityUserFlow setApiConnectorConfiguration:apiConnectorConfiguration];

NSError *error;
NSData *b2cIdentityUserFlowData = [b2cIdentityUserFlow getSerializedDataWithError:&error];
[urlRequest setHTTPBody:b2cIdentityUserFlowData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```