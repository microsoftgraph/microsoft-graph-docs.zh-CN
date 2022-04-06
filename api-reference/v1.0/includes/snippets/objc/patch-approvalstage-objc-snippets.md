---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1856cece4e0de70d135c985631e139c6d2ea7a8e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516058"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/stages/d4fa4045-4716-436d-aec5-57b0a713f095"]]];
[urlRequest setHTTPMethod:@"PATCH"];

MSGraphApprovalStage *approvalStage = [[MSGraphApprovalStage alloc] init];
[approvalStage setReviewResult:@"Approve"];
[approvalStage setJustification:@"OK"];

NSError *error;
NSData *approvalStageData = [approvalStage getSerializedDataWithError:&error];
[urlRequest setHTTPBody:approvalStageData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```