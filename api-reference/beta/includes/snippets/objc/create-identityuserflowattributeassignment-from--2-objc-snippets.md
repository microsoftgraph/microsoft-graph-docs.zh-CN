---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 580b0447835475814df2acc4b58ce3ddf5ac3b5d480f371a2188ab4c41b638f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105880"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlowAttributeAssignment *identityUserFlowAttributeAssignment = [[MSGraphIdentityUserFlowAttributeAssignment alloc] init];
[identityUserFlowAttributeAssignment setIsOptional: false];
[identityUserFlowAttributeAssignment setRequiresVerification: false];
[identityUserFlowAttributeAssignment setUserInputType: [MSGraphIdentityUserFlowAttributeInputType textBox]];
[identityUserFlowAttributeAssignment setDisplayName:@"Shoe size"];
NSMutableArray *userAttributeValuesList = [[NSMutableArray alloc] init];
[identityUserFlowAttributeAssignment setUserAttributeValues:userAttributeValuesList];
MSGraphIdentityUserFlowAttribute *userAttribute = [[MSGraphIdentityUserFlowAttribute alloc] init];
[userAttribute setId:@"extension_guid_shoeSize"];
[identityUserFlowAttributeAssignment setUserAttribute:userAttribute];

NSError *error;
NSData *identityUserFlowAttributeAssignmentData = [identityUserFlowAttributeAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityUserFlowAttributeAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```