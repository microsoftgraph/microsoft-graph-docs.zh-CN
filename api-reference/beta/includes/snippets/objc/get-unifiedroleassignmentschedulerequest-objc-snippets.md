---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efcb92a15e5ff7224f9669eb66c1ca2956746cee223ccada6dcd1b195e76f964
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158445"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleAssignmentScheduleRequest *unifiedRoleAssignmentScheduleRequest = [[MSGraphUnifiedRoleAssignmentScheduleRequest alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```