---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31343073ff5d23a85711658b6949bf64002d58bb
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844381"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
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