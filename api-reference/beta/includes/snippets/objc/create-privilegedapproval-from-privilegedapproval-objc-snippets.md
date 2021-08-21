---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 350589323a9dc09361a99af4d5b35ca8bb869e25b65e459a3549b2e28a39821e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105611"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/privilegedApproval"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphPrivilegedApproval *privilegedApproval = [[MSGraphPrivilegedApproval alloc] init];
[privilegedApproval setUserId:@"userId-value"];
[privilegedApproval setRoleId:@"roleId-value"];
[privilegedApproval setApprovalType:@"approvalType-value"];
[privilegedApproval setApprovalState: [MSGraphApprovalState pending]];
[privilegedApproval setApprovalDuration:@"datetime-value"];

NSError *error;
NSData *privilegedApprovalData = [privilegedApproval getSerializedDataWithError:&error];
[urlRequest setHTTPBody:privilegedApprovalData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```