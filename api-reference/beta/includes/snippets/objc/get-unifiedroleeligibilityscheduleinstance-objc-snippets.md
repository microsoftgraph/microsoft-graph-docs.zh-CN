---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bcc647109c113322fe82785f9efc39605007e14
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474521"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/roleManagement/directory/roleEligibilityScheduleInstances/5cfd7709-7709-5cfd-0977-fd5c0977fd5c"]]];
[urlRequest setHTTPMethod:@"GET"];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        MSGraphUnifiedRoleEligibilityScheduleInstance *unifiedRoleEligibilityScheduleInstance = [[MSGraphUnifiedRoleEligibilityScheduleInstance alloc] initWithData:data error:&nserror];

}];

[meDataTask execute];

```