---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d06aabd6f415159d026d13403dc020abcd8454c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943222"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentRequests"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageAssignmentRequest *accessPackageAssignmentRequest = [[MSGraphAccessPackageAssignmentRequest alloc] init];
[accessPackageAssignmentRequest setRequestType:@"AdminAdd"];
MSGraphAccessPackageAssignment *accessPackageAssignment = [[MSGraphAccessPackageAssignment alloc] init];
[accessPackageAssignment setTargetId:@"46184453-e63b-4f20-86c2-c557ed5d5df9"];
[accessPackageAssignment setAssignmentPolicyId:@"2264bf65-76ba-417b-a27d-54d291f0cbc8"];
[accessPackageAssignment setAccessPackageId:@"a914b616-e04e-476b-aa37-91038f0b165b"];
[accessPackageAssignmentRequest setAccessPackageAssignment:accessPackageAssignment];

NSError *error;
NSData *accessPackageAssignmentRequestData = [accessPackageAssignmentRequest getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageAssignmentRequestData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```