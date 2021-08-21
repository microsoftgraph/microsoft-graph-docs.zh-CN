---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b2f6678190dd1ce5eab8f21a1392e396e3b89a623eff49d298f6dc32331a7ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219420"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleAssignmentSchedules/b1477448-2cc6-4ceb-93b4-54a202a89413"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleAssignmentSchedule *unifiedRoleAssignmentSchedule = [[MSGraphUnifiedRoleAssignmentSchedule alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```