---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d00c7e8734776595c7691d5be73a5e8c8607b4f8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205354"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentSchedules/95c690fb-3eb3-4942-a03f-4524aed6f31e"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleAssignmentSchedule *unifiedRoleAssignmentSchedule = [[MSGraphUnifiedRoleAssignmentSchedule alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```