---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61c32a7c4b17e463887c46d41e23b055e169e60e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690191"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/applications/bcd7c908-1c4d-4d48-93ee-ff38349a75c8/federatedIdentityCredentials/15be77d1-1940-43fe-8aae-94a78e078da0"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphFederatedIdentityCredential *federatedIdentityCredential = [[MSGraphFederatedIdentityCredential alloc] init];
[federatedIdentityCredential setName:@"testing02"];
[federatedIdentityCredential setIssuer:@"https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0"];
[federatedIdentityCredential setSubject:@"a7d388c3-5e3f-4959-ac7d-786b3383006a"];
[federatedIdentityCredential setDescription:@"Updated description"];
NSMutableArray *audiencesList = [[NSMutableArray alloc] init];
[audiencesList addObject: @"api://AzureADTokenExchange"];
[federatedIdentityCredential setAudiences:audiencesList];

NSError *error;
NSData *federatedIdentityCredentialData = [federatedIdentityCredential getSerializedDataWithError:&error];
[urlRequest setHTTPBody:federatedIdentityCredentialData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```