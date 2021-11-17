---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6a735110809ec3072962f4887d10c5da7d790fb259f3b7e165cd1d97bd427da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158661"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageAssignmentPolicy *accessPackageAssignmentPolicy = [[MSGraphAccessPackageAssignmentPolicy alloc] init];
[accessPackageAssignmentPolicy setAccessPackageId:@"56ff43fd-6b05-48df-9634-956a777fce6d"];
[accessPackageAssignmentPolicy setDisplayName:@"direct"];
[accessPackageAssignmentPolicy setDescription:@"direct assignments by administrator"];
[accessPackageAssignmentPolicy setAccessReviewSettings: null];
MSGraphRequestorSettings *requestorSettings = [[MSGraphRequestorSettings alloc] init];
[requestorSettings setScopeType:@"NoSubjects"];
[requestorSettings setAcceptRequests: true];
NSMutableArray *allowedRequestorsList = [[NSMutableArray alloc] init];
[requestorSettings setAllowedRequestors:allowedRequestorsList];
[accessPackageAssignmentPolicy setRequestorSettings:requestorSettings];
MSGraphApprovalSettings *requestApprovalSettings = [[MSGraphApprovalSettings alloc] init];
[requestApprovalSettings setIsApprovalRequired: false];
[requestApprovalSettings setIsApprovalRequiredForExtension: false];
[requestApprovalSettings setIsRequestorJustificationRequired: false];
[requestApprovalSettings setApprovalMode:@"NoApproval"];
NSMutableArray *approvalStagesList = [[NSMutableArray alloc] init];
[requestApprovalSettings setApprovalStages:approvalStagesList];
[accessPackageAssignmentPolicy setRequestApprovalSettings:requestApprovalSettings];

NSError *error;
NSData *accessPackageAssignmentPolicyData = [accessPackageAssignmentPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageAssignmentPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```