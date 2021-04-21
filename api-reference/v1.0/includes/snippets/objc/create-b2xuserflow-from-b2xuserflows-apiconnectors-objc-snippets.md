---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d4daca886b694bb807534b16d798f6f1285cb23
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920288"
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