---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f77237d0408cf438fbc0b917821b16f4d476c198d6b3c49fac5ab6bdf9d03a37
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164254"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleAssignmentMultiple *unifiedRoleAssignmentMultiple = [[MSGraphUnifiedRoleAssignmentMultiple alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```