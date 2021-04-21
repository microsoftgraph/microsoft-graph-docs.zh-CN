---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e30b2afc1056b179169f794e93898161b029d934
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920604"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identity/b2xUserFlows/{b2xIdentityUserFlowId}/userAttributeAssignments/{id}"]]];
[urlRequest setHTTPMethod:@"PATCH"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphIdentityUserFlowAttributeAssignment *identityUserFlowAttributeAssignment = [[MSGraphIdentityUserFlowAttributeAssignment alloc] init];
[identityUserFlowAttributeAssignment setUserInputType: [MSGraphIdentityUserFlowAttributeInputType textBox]];

NSError *error;
NSData *identityUserFlowAttributeAssignmentData = [identityUserFlowAttributeAssignment getSerializedDataWithError:&error];
[urlRequest setHTTPBody:identityUserFlowAttributeAssignmentData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```