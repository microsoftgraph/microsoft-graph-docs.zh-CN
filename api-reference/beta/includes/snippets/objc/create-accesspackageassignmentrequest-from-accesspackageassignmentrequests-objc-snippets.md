---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8b840ee58c7432362a3e8b25b88b85758b42bc8
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473615"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageAssignmentRequest *accessPackageAssignmentRequest = [[MSGraphAccessPackageAssignmentRequest alloc] init];
[accessPackageAssignmentRequest setRequestType:@"UserAdd"];
MSGraphAccessPackageAssignment *accessPackageAssignment = [[MSGraphAccessPackageAssignment alloc] init];
[accessPackageAssignment setAccessPackageId:@"a914b616-e04e-476b-aa37-91038f0b165b"];
[accessPackageAssignmentRequest setAccessPackageAssignment:accessPackageAssignment];
[accessPackageAssignmentRequest setJustification:@"Need access to New Hire access package"];

NSError *error;
NSData *accessPackageAssignmentRequestData = [accessPackageAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```