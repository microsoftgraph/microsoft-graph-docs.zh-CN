---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfe082d62d93865ae5e36c11c95db47cfc5cf13a
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60558734"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/1618dfb0-3ff2-4edf-8d5c-b8f81df00e80/resources"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphEducationAssignmentResource *educationAssignmentResource = [[MSGraphEducationAssignmentResource alloc] init];
[educationAssignmentResource setDistributeForStudentWork: false];
MSGraphEducationResource *resource = [[MSGraphEducationResource alloc] init];
[resource setDisplayName:@"homework example.PNG"];
[resource setFileUrl:@"https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF"];
[educationAssignmentResource setResource:resource];

NSError *error;
NSData *educationAssignmentResourceData = [educationAssignmentResource getSerializedDataWithError:&error];
[urlRequest setHTTPBody:educationAssignmentResourceData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```